## 安装步骤

- **安装Vscode扩展**  

    正式发布前通过VSIX文件进行安装, 先通过下面链接下载clicknium-0.0.1.vsix  
    <a href="https://github.com/k-saihua/clicknium-docs-test" target="_blank">clicknium-0.0.1.vsix</a>  

    ![avatar](/img/vsce-install.png)

- **安装python sdk**  
    在vscode中开发python，建议先安装Microsoft Python Extension  

    ![avatar](/img/pye-install.png)

- **安装浏览器扩展**  
    在vscode terminal或者命令行下运行python  
    然后运行以下命令  
    ```python
        >>> from clicknium import clicknium as cc
        >>> cc.chrome.extension.install()
    ```
    **安装成功之后，打开浏览器手动启用扩展，然后刷新浏览器或者重新打开浏览器，扩展生效**  

## 第一个项目

- **创建或者打开vscode项目**   

- **录制元素**   

- **查看和编辑验证选择器**   

- **新建python文件，编写流程**  
    ```python
    from clicknium import clicknium as cc, selectorstore

    #操作一个已经打开的浏览器
    cc.find_element(selectorstore.chrome.baidu.text_kw).set_text("rpa")
    cc.find_element(selectorstore.chrome.baidu.submit_su).click()

    #打开一个浏览器操作
    driver = cc.chrome.open("www.baidu.com")
    driver.find_element(selectorstore.chrome.baidu.text_kw).set_text("rpa")
    driver.find_element(selectorstore.chrome.baidu.submit_su).click()
    driver.close()
    ```

- **运行流程**  