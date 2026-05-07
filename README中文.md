# 说明文档 - 如何使用此存储库

## 装入你的面包
1) 开始前请加载到您的分支
- 如果是第一次，请执行以下操作
   ```
   python -m venv venv
   ```
   ```
   source venv/bin/activate 
   ```
   ```
   pip install requirements.txt 
   ```

- 环境设置完成后（您正在继续工作）：
    - 如果您在终端中看不到 (venv) 和您的名字（应该是您的名字而不是 (tutorial)），就像图片中显示的那样。

     ![image](https://github.com/hivan04/ml-finance/blob/tutorial/explanation_images/1.png)
  <br>

   Do the following:
   ```
   git switch your_name
   ```
   ```
   source venv/bin/activate 
   ```

## 正在更新您的存储库
2) 要对您的代码仓库进行任何更改/更新，请执行以下操作（**请确保您已保存要上传的文件**）：
**请确保您当前位于您的分支中**<br>

![image](https://github.com/hivan04/ml-finance/blob/tutorial/explanation_images/2.png)<br>

*You can check yourself by running the following (you should see an * next to your name if you are in your branch)*
   ```
   git branch
   ```
   
- If you just want to update everything (easiest method for updating repository)
   ```
   git add .
   git commit -m "write something here"
   git push
   ```

- 如果您只想上传特定文件，请不要使用“.”，而是输入文件路径名。
    ```
      git add '/put_pathname_here'
      git commit -m "write something here"
      git push
      ```

## 从存储库拉取
如果您想从特定分支拉取文件（例如，您想拉取课程作业的 PDF 文件并将其添加到您的分支），
- 再次提醒，请确保您位于您的分支中：
      ```
      git switch 'your_name' 
      git branch
      ```
然后运行以下命令 (*path/to/file is the file you want to copy into your branch, e.g.: misc/Dividend_Signal_Alpha_Coursework_Final.pdf*)
      ```
      git fetch 
      git checkout main -- path/to/file
      git add path/to/file
      git commit -m "copy file from main"
      git push
      ```