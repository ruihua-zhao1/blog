# Simulate view port

 - await page.setViewport({width:1650, height:1050})
 - await page.goto('http://www.baidu.com')
  
# Simulate tablet

  - const tablet = puppeteer.devices['iPad landscape']
  -  await page.emulate(tablet)
  -  await page.goto('http://www.baidu.com')
  
# Simulate mobile device

  - const mobile = puppeteer.devices['iPhone X']
  - await page.emulate(tablei)
  - await page.goto('http://www.baidu.com')