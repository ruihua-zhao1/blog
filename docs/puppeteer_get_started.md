# Get start
 - Const browser = await puppeteer.launch({
    headless: false,
    slowMo: 500，
    devtools: true
    })
  - sloeMo 延迟0.5秒执行
  - devTools :可以打开developer tools
  - browser.newPage()
  - page.setDefaultTimeout(6000)
  - page.waitForSelector('#sss')
  - page.click('#aaa')
  - page.waitForXpath('//a')
  
# Basic command
Here is the basic command for puppeteer:
  - page.waitForSelector
  - page.click(‘#aa’, clickCount: 5)
  - Dropdown下拉框：page.select()

  - const text = await page.@eval(‘#aaa’, element => element.textContent)
  - const a = await page.$$eval(‘p’, element => element.length)
  
Wait for element disappear:
  - await page.waitfor(()=>!document.querySelector(‘#sss’))
  - await page.waitForSelector(‘#sss’, {hidden: true, timeout: 100})