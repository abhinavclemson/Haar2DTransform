
# Basic image convolution and edge detection


	Name: ABHINAV SINGH 
	COURSE ID : CPSC-6820 
	Section number :003 


## Background 

**DWT transform**

**Haar Wavelet Transform:**

It involves forward and reverse transforms:

1. Forward Transform:
 * 	Computation of scaling coefficients- add two adjacent and sample values and divide by 2.
 *  Computation of wavelet coefficients-subtract two adjacen sample values and divide by 2.
2.  Inverse Transform:
	* Computation requires simply addition and subtraction.
	

User can provide levels to the DWT module as well as levels to the Inverse DWT  module to see how the Image restoration is going bottom-up.


##Steps in program
1. An image input is given that is of **ppm** type, which is in RGB colored type and has pixel values between 0-255.
2. The image is converted into grey scale **pgm** type image in 2D array.
3. Its values are copied in a 2-D array of float type.
4. Converting length of image height and width into powers of 2s.
5. Haar wavelet transform on the image array, which now has length and height in powers of 2s.
6. The output unnormalized image array is saved into "dgrey.pgm".
7. The unnormalized image array is copied for normalizing it between 0-255 and saved to "ngrey.pgm".
8. The unnormalized image array is then passed into Inverse Haar wavelet transform module, it is restored to the provided level in a bottom-up approach.
9. The Inverse Haar wavelet tranformed array is then saved to "grey.pgm".






## Instructions for the user
1. Program is written in Jupyter notebook using python 3.x
2. Original file is in .ipynb format to open it in Jupyter notebook.
3. Additional, .py files are are also attached, if the user wants to open it in python interpreter.
4. As the program is made on Macos, it uses forward slash for accessing directories, and would automatically detect the directory by using os.cwd for getting present working directory. Have to change forward slash to backward slash , if user operating on Windows machine. 
5. backward slash used in ppm*_*write and pgm*_*write, specifically for the variable **file**.
6. for windows user:

           file= os.getcwd()+'/Output/'+file_name
           can be changed to
           file= os.getcwd()+'\Output\'+file_name
7. Comments are provided in the files. Additionally, code snippets are also provided to show results of previous run.
8. for jupyter notebook file(.ipynb), Image address to be manually inserted while running it.
9. for Python file(.py), in command line image address to be inserted.</br>
	command: python3  < python file>  < filename>.</br>
	for example: </br>
	python DWT.py Images/mandrill.ppm
10. Program would ask for number of levels and inverse levels. Inverse levels are the levels to which the user want the image to be restored, if no input is provided, image would be restored to its former-self.

	
	
	




           
## Dependencies
* [Python 3.0.x](https://www.python.org/download/releases/3.0/)
* [NumPy](https://numpy.org/)
* [Pillow](https://pillow.readthedocs.io/en/stable/)


## Technologies
* [Jupyter notebook](https://jupyter.org/)
* Can be used on **Idle**  too.



Both Jupyter notebook file(.ipynb) and python file(.py) is provided.

           

