Here’s the small assignment. Do all of the 10 questions, most of them are very easy, and create a Jupyter notebook with all the commands you ran for each question. We will meet next Tuesday, same time 4:00 PM to 5:00PM. Please bring your laptops.

Please navigate to for a better markdown format of the questions written below.
 
In your machines:

1. Create a folder named `linux_assignment` in your home folder (using `mkdir`).
2. Download this dataset (http://www.vision.caltech.edu/Image_Datasets/faces/faces.tar) by using `wget`. 
3. Create a folder inside `linux_assignment` for the dataset and name it `face_dataset`.
4. Untar the contents of the downloaded dataset after going into `face_dataset`.
5. Find the number of files in the folder. (remember `wc` ? - do `ls | wc -l`).
6. Find the number of `jpg` images in the folder. ( do a `find -name ...` command or `ls *….` ).
7. Install the program named `parallel` in your machine - `sudo apt-get install parallel`. You’ll be asked for a password, ask me the password beforehand in Slack :)
8. Convert all the `jpg` files to `tiff` format using `convert` command and `parallel` module. This is where you should be careful. If you mess it up, just delete the files, untar the downloaded file again and redo :) Reach out to me if you are stuck. It is the same command we went through, but instead of converting from `jpg` to `tiff`, here we are doing reverse. For example, you can use `find`, `parallel` and `convert` piped together. NOTE: sometimes, you will end up with both `jpg` and `tiff`. In that case, please delete the `jpg` files using `rm` command (`rm *….`).
9. Use `sed` to replace all instances of the word `image` to `IMAGE` inside the `README` file. For example, `sed -i s/'old-string’/'new-string'/g`.
10. Use `zip` to compress the extracted folder (you might want to go down one level in folder structure), now with all the tiff images, and save it as `face_images_tiff.zip`. Remember the `zip` convention we discussed yesterday - `zip zipped_file_name.zip folder_to_zip`.

As I mentioned, please let me know if you are stuck. Reach out in Slack `general` channel so that anyone who knows how to do it can reply :) You could always send a message to me as well if you prefer so. Google if you have doubts and try to figure it out. As we discussed, manual pages for all of the commands can be found by typing `man name_of_command` for example - `man convert`.

Hope you’ll learn something new :)
