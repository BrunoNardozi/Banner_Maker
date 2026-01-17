This is a simple python project created with the aim of streamlinning the process of adding information banners to real state photos. 

It's composed by 3 blocks of code.

Excel Reader: reads and prepares the information to be inserted on the banners from an excel file  
Image Maker: takes the information from the excel and creates a new image with the banners  
Folder Processor: takes a mother folder and creates a copy with bannered photos inside  


How to use: 

Prepare the excel with your information. 

Column A: ref - your internal reference (should match folder name)  
Column B: typology - house, store, apartment, etc  
Column C location - where is the real state located  
Column D: price - price in Euros  
Column E: area - total area in m2  
ColumnF: bedrooms - number of bedrooms

In SETUP add paths to:  
excel_path - path to provided excel  
image_path - path to image (define this only if you want to process a single image)  
program_folder - path to Icons folder (Icons should be named "ref.png", "typology.png", "location.png", "price.png", "area.png" and "bedrooms.png")  
font_path - path to .ttf font  
ref - ref of your image (define this only if you want to process a single image)  
banner_size - size of the banner (default is 0.1)  
mother_folder - path to mother folder

Run the three code blocks and call image_maker to process a single image OR call folder_processor to process all images in a folder system where folder names correspond to ref in excel
