# Animations

## keyframes
Create keyframes
```
@keyframes drive{
  from{ transform: translateX(-150px) }
  to{ transform: translateX(1800px) }
}
@keyframes jump{
  0%{ top: -40px }
  50%{ top: -100px }
  100%{ top: -40px }
}
```
Call the keyframes
```
animation-name: drive;
animation-duration: 5s;
animation-fill-mode: both;
animation-iteration-count: infinite;
animation-timing-function: linear;
```
or
```
animation: drive 5s both infinite linear;
```