---


---

<p>IV. Розробка та налагодження програмного забезпечення та супровідної документації.</p>
<ol>
<li>
<p>ПЗ для Edge-рівня.</p>
</li>
<li>
<p>Схеми інформаційної взаємодії.</p>
</li>
<li>
<p>ПЗ для хмарних рішень.</p>
</li>
<li>
<p>WEB-інтерфейси (локальний для Edge та глобальний).</p>
</li>
</ol>
<h1 id="розділ-4.-розробка-та-налагодження-програмного-забезпечення-та-супровідної-документації.">Розділ 4. Розробка та налагодження програмного забезпечення та супровідної документації.</h1>
<h1 id="пз-для-edge-рівня.">ПЗ для Edge-рівня.</h1>
<p>ПЗ розроблено в середовищі Node-RED (яке запускається автоматично з запуском Raspberry PI)</p>
<p>Застосунок включає кілька потоків (Flow):</p>
<ul>
<li>
<p>process - для обробки і імітації змінних</p>
<p>![image-20200605172611056](file://C:/Users/user/AppData/Roaming/Typora/typora-user-images/image-20200605172611056.png?lastModify=1591368620)</p>
</li>
<li>
<p>UI - для роботи з локальним ВЕБ-інтерфейсом</p>
<p>![image-20200605172602089](file://C:/Users/user/AppData/Roaming/Typora/typora-user-images/image-20200605172602089.png?lastModify=1591368620)</p>
</li>
</ul>
<p>![image-20200605172542020](file://C:/Users/user/AppData/Roaming/Typora/typora-user-images/image-20200605172542020.png?lastModify=1591368620)</p>
<ul>
<li>History - для роботи з локальною базою даних для збереження даних</li>
</ul>
<p>![image-20200605172536049](file://C:/Users/user/AppData/Roaming/Typora/typora-user-images/image-20200605172536049.png?lastModify=1591368620)</p>
<ul>
<li>Alarm - для роботи з тривогами</li>
</ul>
<p>![image-20200605172532437](file://C:/Users/user/AppData/Roaming/Typora/typora-user-images/image-20200605172532437.png?lastModify=1591368620)</p>
<ul>
<li>Bot - для роботи з чат-ботом Telegram</li>
</ul>
<p>![image-20200605172512926](file://C:/Users/user/AppData/Roaming/Typora/typora-user-images/image-20200605172512926.png?lastModify=1591368620)</p>
<p>![image-20200605172524374](file://C:/Users/user/AppData/Roaming/Typora/typora-user-images/image-20200605172524374.png?lastModify=1591368620)</p>
<ul>
<li>Report - для формування звітів та взаємодії з Google Sheet</li>
</ul>
<p>image-20200605172334940</p>
<p>Система передбачає взаємодію через глобальні контексти Node-RED. Передбачено наступні глобальні контексти:</p>
<ul>
<li>
<p>RTDB - для збереження конфігураційних та плинних даних вимірювання та керування та трендів на останню хвилину</p>
</li>
<li>
<p>ALM - для збереження конфігураційних даних для налаштування тривог та стану тривог</p>
</li>
<li>
<p>RPRT - для збереження буферу для формування звітів</p>
</li>
</ul>
<p><strong>Схеми інформаційної взаємодії</strong></p>
<p><strong>ПЗ для хмарних рішень</strong></p>
<ul>
<li>
<p>Налаштування Google Sheet</p>
<p>![image-20200605172323734](file://C:/Users/user/AppData/Roaming/Typora/typora-user-images/image-20200605172323734.png?lastModify=1591368620)</p>
</li>
<li>
<p>Налаштування Telegram</p>
</li>
</ul>
<p><strong>WEB-інтерфейси (локальний для</strong>  <strong>Edge</strong>  <strong>та глобальний)</strong></p>
<ul>
<li>
<p>зовнішній вигляд локального WEB-інтерфейсу</p>
</li>
<li>
<p>опис потоку UI</p>
</li>
<li>
<p>зовнішній вигляд та опис інтерфейсу глобального Веб-інтерфейсу</p>
<p>![image-20200605172245199](file://C:/Users/user/AppData/Roaming/Typora/typora-user-images/image-20200605172245199.png?lastModify=1591368620)</p>
</li>
</ul>

