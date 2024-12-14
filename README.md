# Студент группы М8О-408Б-21 Королев И.С.

---

[main.ipynb](https://github.com/Kiyoakiii/ML_mai/blob/main/main.ipynb) - содержит лабораторные работы 1-5 по курсу "Методы, средства и технологии мультимедиа"

---

<div align="center" style="font-family: Arial; background-color: #f0f0f0; padding: 40px; border-radius: 10px; width: 60%; margin: auto;">
  <span style="font-style: italic; color: #333;">В следующей таблице в ячейках, относящихся к классификации я буду отображать <strong>accuracy</strong>; в ячейках, относящихся к регрессии я буду отображать <strong>MSE</strong></span>
  <br>
  <span style="font-style: italic; color: #333;">*Метрика качества на тестовом наборе данных*</span>
  <table border="1" cellpadding="10">
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
  <th rowspan="1" style="padding: 10px; border: 1px solid #ddd; background-color: #0099cc; color: white;">Алгоритм</th>
  <th style="padding: 10px; border: 1px solid #ddd; background-color: #0099cc; color: white;">Задача</th>
  <th style="padding: 10px; border: 1px solid #ddd; background-color: #0099cc; color: white;">Бейзлайн</th>
  <th style="padding: 10px; border: 1px solid #ddd; background-color: #0099cc; color: white;">Улучшенный бейзлайн</th>
  <th style="padding: 10px; border: 1px solid #ddd; background-color: #0099cc; color: white;">Самостоятельная имплементация алгоритма</th>
  </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td rowspan="2">KNN</td>
      <td>классификация</td>
      <td style="color: #9c0006;">0.9025</td>
      <td style="color: #006100;">0.91</td>
      <td style="color: #006100;">0.91</td>
    </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td>регрессия</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.025</td>
      <td style="background-color: #00BFFF30; color: #006100;">0.0237</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.0246</td>
    </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td rowspan="2">Линейные модели</td>
      <td>классификация</td>
      <td style="color: #9c0006;">0.753</td>
      <td style="color: #006100;">0.75375</td>
      <td style="color: #006100;">0.75375</td>
    </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td>регрессия</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.0729599</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.072958</td>
      <td style="background-color: #00BFFF30; color: #006100;">0.0729595945</td>
    </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td rowspan="2">Решающее дерево</td>
      <td>классификация</td>
      <td style="color: #006100;">0.80375</td>
      <td style="color: #006100;">0.80875</td>
      <td style="color: #9c0006;">0.8075</td>
    </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td>регрессия</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.0487121</td>
      <td style="background-color: #00BFFF30; color: #006100;">0.046489</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.07423</td>
    </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td rowspan="2">Случайный лес</td>
      <td>классификация</td>
      <td style="color: #9c0006;">0.9025</td>
      <td style="color: #006100;">0.905</td>
      <td style="color: #9c0006;">0.8875</td>
    </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td>регрессия</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.0242</td>
      <td style="background-color: #00BFFF30; color: #006100;">0.0231</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.065</td>
    </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td rowspan="2">Градиентный бустинг</td>
      <td>классификация</td>
      <td style="color: #9c0006;">0.87</td>
      <td style="color: #006100;">0.905</td>
      <td style="color: #9c0006;">0.8525</td>
    </tr>
    <tr style="background-color: #f2f2f2; text-align: center; font-weight: bold; color: #333;">
      <td>регрессия</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.056177</td>
      <td style="background-color: #00BFFF30; color: #006100;">0.04029</td>
      <td style="background-color: #00BFFF30; color: #9c0006;">0.0847192</td>
    </tr>
  </table>
    <h2 style="color: #333; text-align: center; font-weight: bold;">Выводы:</h2>
    <ul style="font-size: 18px; color: #555; line-height: 1.6;">
        <li><strong>KNN и Случайный лес</strong> продемонстрировали стабильно высокие результаты как в классификации, так и в регрессии.</li>
        <li>Для классификации стоит предпочесть <strong>KNN</strong>, так как он показал наилучший <span style="color: #00BFFF;">accuracy</span> среди всех алгоритмов.</li>
        <li>Для регрессии <strong>Случайный лес</strong> обеспечил наилучший результат по метрике <span style="color: #ff6347;">MAE</span>, что делает его наиболее подходящим для этой задачи.</li>
    </ul> 
</div>
