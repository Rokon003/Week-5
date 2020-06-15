import urllib.request, urllib.parse, urllib.error
import xml.etree.ElementTree as ET

url=input("Enter: ")
uo=urllib.request.urlopen(url).read()

tree=ET.fromstring(uo)
list=tree.findall('comments/comment')

count=0
sum=0

for item in list:
    x=item.find('count').text
    count=count+1
    sum=sum+int(x)

print("count: ", count)
print("sum: " , sum)
    
