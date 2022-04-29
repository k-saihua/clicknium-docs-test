# 开始

- **简单的使用**  

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

- **实例分析**