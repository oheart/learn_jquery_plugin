## perspective属性（近大远小）两种书写方式
（1）用在3D元素父亲上
```css
.ct{
    perspective: 200px;
}
```
（2）用在当前3d元素上，与transform的其他属性写在一起。
```css
#ct .box{
    transform: perspective(200px) rotateY(45deg);
}
```
## perspective-origin
perspective-origin定义了元素的位置，默认是3d容器的中心。  
当为元素定义perspective-origin属性时，其子元素会获得透视效果，而不是元素本身。  
该属性必须与perspective属性一同使用，而且只影响3D转换元素，如perspective-origin: 10% 10%;    
设置`backface-visibility:hidden`，看不见元素的背面。  
## transform-style: preserve-3d

