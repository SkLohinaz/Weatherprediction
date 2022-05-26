# Weatherprediction
import requests
city = input('Enter City name: ')
print('Displaying Weater report for: ' + city)
url = 'https://wttr.in/{}'.format(city) 
res = requests.get(url)                 
print(res.text)
