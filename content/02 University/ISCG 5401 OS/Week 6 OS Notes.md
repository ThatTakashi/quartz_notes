[[File Paths.canvas|File Paths]]

## Revision Questions:
### Q1: Using absolute path, go to the folder OSF from Home.
cd /Home/University/OSF

### Q2: Go to the Root directory from Home.
cd ..

### Q3: From the Soccer directory, use relative path to create a new text file called Yellow.txt in the folder Game1. Insert the text “Hello” as the content of Yellow.txt.
echo "Hello" ../../../Game/Game1/Yellow.txt

### Q4: From OSF, use relative path to display the content of the file NZ.txt.
cat ../../Sport/Team/Rugby/NZ.txt

### Q5: From the Counter directory, use absolute path to duplicate the file NZ.txt in the Home directory and call it Black.txt.
cp /Home/Sport/Team/Rugby/NZ.txt /Home/Black.txt

### Q6: From the Test1 directory, use relative path to create a folder in the League directory called New.
mkdir ../../../Sport/Team/Soccer/League/New