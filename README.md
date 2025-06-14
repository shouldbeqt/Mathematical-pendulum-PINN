<div align = "centre">
  
# This repositories demostrate PDE solution of mathematical pendulum by PINN

</div>

By mathematical pendulum i try to explore PINN and neural networks, so this solution can not be clear right, but result which i get was satisfying

---

1. Like in default PINN i put PDE in loss function

2. Inital condition was just as standart when t = 0

3. But for boundary condition i using analytics formul for period, but it is created with approximation sin(a) ~ a, so i choose small max angle for smooth out this approximation

![PINN](https://github.com/user-attachments/assets/17120714-55d4-4aeb-b743-e0fc7343563e)

So i get so simple model due to learning taken around 10-20 minutes, and i recomend using your GPU for computate models

MSE LOSS (on control points, which are locate t = T, t = 0, t= T/2, t=3T/4, t=T/4, comapre model angle predict), i get less 1 procent

**If someone wants to upgrate model, i recomend using Neumann condition d(angle)/dx**
