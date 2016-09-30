# Shell-Scripts
mkpics - Writes to standard output HTML code that displace a table of photos. The first command line argument is the number of columns in the table, and remaining arguments are the files to be displayed.
For example:

!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
<html>
  <head>
    <title>Pictures</title>
  </head>

  <body>
    <h1>Pictures</h1>

<table>
<tr> 
<td><img src="pictures/IMGP0959.jpg" height=100></td> 
<td><img src="pictures/IMGP2739.jpg" height=100></td> 
<td><img src="pictures/IMGP2850.jpg" height=100></td> 
</tr> 
<tr> 
<td><img src="pictures/IMGP3064.jpg" height=100></td> 
<td><img src="pictures/IMGP3069.jpg" height=100></td> 
<td><img src="pictures/IMGP3528.jpg" height=100></td> 
</tr> 
</table>
</body> </html> 

filepics - Takes an existing directory as an argument, for each picture in the directory, it takes the date the picture was generated. It then creates years as directories, and months as subdirectories in each year folder.

mkpics2 - A modified mkpics, takes number of columns and a directory as an argument. The directory should be the root of a folder that had filepics run on it. It then outputs HTML code with a table of photos for each year.
For example:

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
<html>
  <head>
    <title>Pictures</title>
  </head>

  <body>
    <h1>Pictures</h1>

<h2>2012</h2>
<table>
<tr> 
<td><img src="2012/01/IMGP2739.jpg" height=100></td> 
</tr> 
</table>

<h2>2011</h2>
<table>
<tr> 
<td><img src="2011/01/IMGP2850.jpg" height=100></td> 
<td><img src="2011/03/IMGP3064.jpg" height=100></td> 
</tr> 
<tr> 
<td><img src="2011/03/IMGP3069.jpg" height=100></td> 
</tr> 
</table>
</body> </html> 
