This repository will contains 3D IC files that I extracted from the https://asignin.space/ simulation with the help of #asigninspace community.

You can import them in a 3D software to view them.

Method for obtain 3D IC view from a image decoded from ASignInSpace simulation (https://asignin.space):

1) Aligned all squares from original_square.png (https://github.com/BatchDrake/ASignInSpace/blob/master/Candidates/visual/original_square.png). I use the exemple png file aligned by "Sparta | Phrenic" user from "A Sign In Space" discord.

2) Extract all RGB value from aligned squares file and compute each bits visual image for 8 bits layers with a python script.

3) With all RGB aligned squares images use "Towards Robust Monocular Depth Estimation: Mixing Datasets for Zero-shot Cross-dataset Transfer", with
"Vision Transformers for Dense Prediction" research for retrieve a very good quality depth image for each with "Inference height 512 MiDaS model" (v3.1 BEiTL-512).

4) Generate pcd files with combinaison of all image and her depth.
Exemple online with this https://imagetostl.com/convert/file/png/to/pcd 

5 ) Merge all pcd files to the merged.pcd file.


