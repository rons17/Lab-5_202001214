# Lab-5_202001214

### Python code for helpRobot

#### def main():
    for _ in range(int(input()))
        (x1, y1, x2, y2) = map(int, input().split())
        if x1 == x2:
            if y2> y1:
                print('up')
            else:
                print('down')
        elif y1 == y2:
            if x2> x1 :
                print('right')
            else:
                print('left')
        else:
            print('sad')

if __name__ == '__main__':
    main()
    
    ### 1) Static Analysis of above python code.
    Errors : semicolon is missing after for loop
    
    ### 2)Static Analysis using pylint tool.
- Pylint tool is used to analyze static code i.e. static functions of the code will be analyzed and errors will be reflected
- While dynamic functions of python (where return variable type is not defined) will not be analyzed for error-checking
- We checked our dummy repository of the project using pylint tool with command 'py -m pylint ./'

 After running this code file in Command promp I get following warning using this tool
 
 ![image](https://user-images.githubusercontent.com/124248015/225589212-112006c9-96ec-47dc-8091-489e477f629d.png)
 
 After Correcting this error I check this file again using pylint tool.
 
 ### Corrected Code: 
 
 #### def main():
    for _ in range(int(input()))
        (x1, y1, x2, y2) = map(int, input().split())
        if x1 == x2:
            if y2> y1:
                print('up')
            else:
                print('down')
        elif y1 == y2:
            if x2> x1 :
                print('right')
            else:
                print('left')
        else:
            print('sad')

if __name__ == '__main__':
    main()

Following are the Outputs of pylint tool 

![image](https://user-images.githubusercontent.com/124248015/225590728-c4d94242-710f-4a3a-b0d5-5708a50470c6.png)

This tool helps me to find and fix errors and display quality issues in my code. 
This tool can also measure various metrics of the code, as shown in image it gives rating of my python code. 
This tool will be integrated into the software development process as part of the code editor in early phase of development.

