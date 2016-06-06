# css line-height
##CSS:line-height:150%与line-height:1.5的真正区别是什么？
```html
<div style="line-height:150%;font-size:16px;">
父元素内容
<div style="font-size:30px;">
Web前端开发<br />
行高问题
</div>
</div>
```
1、当line-height:150%的效果，父元素的行高为150%时，会根据父元素的字体大小先计算出行高值然后再让子元素继承。所以当line-height:150%时，字元素的行高等于16px * 150% = 24px</br>
2、当line-height:1.5em的效果，父元素的行高为150%时，会根据父元素的字体大小先计算出行高值然后再让子元素继承。所以当line-height:1.5em时，子元素的行高等于16px * 1.5em = 24px</br>
3、当line-height:1.5的效果，父元素行高为1.5时，会根据子元素的字体大小动态计算出行高值让子元素继承。所以，当line-height:1.5时，子元素行高等于30px * 1.5 = 45px</br>
