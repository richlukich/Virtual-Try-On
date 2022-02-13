# Virtual-Try-On
Финальный проект первого семестра DLS2021/2022. Суть заключалась сделать виртуальную примерочную. Что-то в духе https://www.clometrica.com/.


Основная часть (пайплайн):
- берется готовый меш одежды
- на вход приходит видео человека в полный 
рост (перед зеркалом/снятого от 3-го лица)
- предсказывается 3D-поза человека 
по этому видео (покадрово)
- далее на каждом кадре видео:
-- поза конвертируется в нужный 
формат для перепозирования 3D 
модели одежды 
-- перепозированный меш одежды 
рендерится (отрисовывается) поверх 
картинки


Результат: 



![github](https://github.com/richlukich/Virtual-Try-On/blob/main/image.gif)


Полезные ссылки:

"1. Статьи на русском про 3DML: https://m.habr.com/ru/company/itmai/blog/503358/

2. Рассказ про моделирование 3D одежды: 
https://youtu.be/ySx-iE-mb0s 

3. Модель камеры: 
http://www.cse.psu.edu/~rtc12/CSE486/lecture12.pdf
http://www.cse.psu.edu/~rtc12/CSE486/lecture13.pdf 

4. Мы будем активно работать с библиотеками:
* pytorch3d: https://pytorch3d.org
* https://pytorch3d.org/tutorials/render_textured_meshes
* open3d: http://www.open3d.org
* [опционально] * pyrender: https://github.com/mmatl/pyrender

5. SMPL: 
* https://www.youtube.com/watch?v=kuBlUyHeV5U
* https://khanhha.github.io/posts/SMPL-model-introduction/ 

6. Предсказание 3D-позы: 
* https://github.com/facebookresearch/frankmocap
* [опционально] https://github.com/vchoutas/expose
* [опционально] https://google.github.io/mediapipe/solutions/pose

7. Датасеты мешей одежды: 
* https://github.com/bharat-b7/MultiGarmentNetwork
* [опционально] https://github.com/jby1993/BCNet 
* [опционально] https://github.com/aymenmir1/pix2surf "
