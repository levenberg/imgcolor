import cv2
import numpy as np
img=cv2.imread('/home/yangpc/workspace/imgcolor/cap1/2880.png')
#cap=cv2.VideoCapture(1)
#while 1:
#       ret,img=cap.read()       
#cv2.pyrDown(img,img)
#img=cv2.medianBlur(img,5)
img_hsv=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
img_br=img[:,:,2]*1.0/(img[:,:,0]+1)#r/b
img_gb=img[:,:,1]*1.0/(img[:,:,0]+1)#g/b
img_rg=abs(img[:,:,2]-img[:,:,1])#r-g
img_y=(img[:,:,2]+img[:,:,1])*1.0/img[:,:,0] # r+g /b
print img_br
img_br=img_br/2
img_gb=img_gb/4
img_rg=img_rg
img_y=img_y*1.0/15
cv2.imshow('r/b',img_y)
cv2.imshow('g/b',img_gb)
cv2.imshow('r-g',img_rg)
cv2.imshow('y',img_y)
cv2.imshow('b',img[:,:,0])
cv2.imshow('g',img[:,:,1])
cv2.imshow('r',img[:,:,2])
cv2.imshow('h',img_hsv[:,:,0])
cv2.imshow('s',img_hsv[:,:,1])
cv2.imshow('v',img_hsv[:,:,2])
cv2.waitKey(0)
