from bs4 import BeautifulSoup
import requests

html_text = requests.get('https://en.wikipedia.org/wiki/Software_engineering').text
soup = BeautifulSoup(html_text,'lxml')
print('The header tags are :')

# list of tags"
headers = ["h1","h2","h3","h4","h5"]
for tags in soup.find_all(headers):

	  print(tags.text.strip().replace('[edit]',''))
