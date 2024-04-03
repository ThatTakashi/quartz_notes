# Task 1:
## Copy File1 to Ssub1 and rename to yourname.txt
*Currently in /Desktop folder*

**cp** File1.txt Sub1/Ssub1/Aidan.txt

## Copy File 1 to Ssub2 with same name (File 1)
*Currently in /Desktop folder*

**cp** File1.txt Sub2/Ssub2

## Display content of File1 from Desktop
*Currently in /Desktop folder*

**cat** File1.txt

## Move File2 to Sub1
*Currently in /Ssub1 folder*

**echo** "Test" File2.txt
**mv** File2.txt ../../Sub2/Ssub2

## Remove Sub1
*Currently in /Desktop folder*

**rm -r** Sub1

# Task 2:
## Move File3 to D_Ssub2 and rename to yourname.txt
*Currently in /D_Ssub1*

**cp** File3.txt ../../Doc_sub2/D_Ssub2/Aidan.txt

## Copy File4 to Document with same name
*Currently in /D_Ssub2*

**cp** File4.txt ../..

## Move D_File2 to Ssub 2 and rename to studentID.txt
*Currently in /Doc_sub1*

**mv** D_File2 D_Ssub2/studentID.txt

## Remove Doc_ Sub2
*Currently in /Document*

**rm -r** Doc_sub2

## Remove Sub_2 and Doc_Sub1
*Currently in /Document*

**rm -r** Doc_sub1