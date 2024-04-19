# Patch Chromedriver
- Install the UndetectedChromeDriver package.
  - `pip3 install undetected_chrome`
- Run the Patcher
  - Provide the path to the unpatched chrome driver in the `driver_executable_path`.
  - Execute the python code and the driver should be pathched.
    ```python
      import undetected_chromedriver as uc
      options = uc.ChromeOptions()
      driver = uc.Chrome(options = options, driver_executable_path="./chromedriver")
      driver.get('https://google.com')
      driver.save_screenshot('nowsecure.png')
    ```
