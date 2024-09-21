# LinkedBot with Selenium and Gemini AI
### Code
Code is in `linkedin.py`
Add a `.env`
```python
GOOGLE_API_KEY  = "YOUR API KEY"
GMAIL = "Your gmail"
PASSWORD = "your Linkein password"
```
Change the post under which you need AI-generated comments. In line 67 in `linkedin.py`
Code line
```python
 driver.get('https://www.linkedin.com/posts/srijaalla_a-couple-of-days-ago-i-went-to-the-doctor-activity-7228914698379796480-ELnQ?utm_source=share&utm_medium=member_desktop')
```
Code block
```python
while(1):
    try:
        driver.get('https://www.linkedin.com/posts/srijaalla_a-couple-of-days-ago-i-went-to-the-doctor-activity-7228914698379796480-ELnQ?utm_source=share&utm_medium=member_desktop')
        win = driver.find_element(By.TAG_NAME, "html")
        driver.execute_script("arguments[0].click();", win)
```
### Add files
Run - 
```python
python -m venv venv
pip install requirements.txt
python linkedin.py
```
