python -m venv flowers 

Goto flowers/script/activate.bat

You should see this (flowers) 

type cd..

pip install -r requirements.txt

Commands for training in Windows:

python -m scripts.retrain   --bottleneck_dir=tf_files/bottlenecks --how_many_training_steps=500   --model_dir=tf_files/models/ --summaries_dir=tf_files/training_summaries/"mobilenet_0.50_224" --output_graph=tf_files/retrained_graph.pb   --output_labels=tf_files/retrained_labels.txt   --architecture="mobilenet_0.50_224"  --image_dir=tf_files/flower_photos

python -m scripts.label_image  --graph=tf_files/retrained_graph.pb --image=tf_files/flower_photos/daisy/21652746_cc379e0eea_m.jpg




