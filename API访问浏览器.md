# python-api
from selenium import webdriver
from time import sleep
aa = webdriver.Firefox()
aa.get("http://www.baidu.com")
aa.find_element_by_id('kw').send_keys('geckodriver')
aa.find_element_by_id('su').click()

# 浏览器最大化
aa.maximize_window()

print("设置浏览器宽480、高800显示")
aa.set_window_size(480, 800)
sleep(2)
aa.close()
