# **ПРАКТИЧНА РОБОТА №14**

## **Тема: Оптимізація зображень за допомогою Squoosh**
## **Мета:**
1. Ознайомити студентів із методами стиснення зображень та їхнім впливом на якість.
2. Навчити визначати оптимальний баланс між якістю та розміром файлу.
3. Ознайомити студентів із різними типами стиснення: без втрат (lossless) та з втратами (lossy).
4. Дослідити вплив зміни розміру на якість зображення та вагу файлу.
5. Навчитися адаптувати зображення для різних цільових застосувань:
- Веб (оптимізація для швидкого завантаження).
- Мобільні пристрої (зменшені розміри, ефективне стиснення).
- Retina-дисплеї (2x, 3x версії для збереження якості).
6. Закріпити навички документування та аналізу результатів у Markdown-форматі у GitHub-репозиторії.

### Хід роботи:

#### **1. Обираємо 3 зображення фото/скріншот/графічне зображеня з текстом:**

**1.Фото**

![model](https://github.com/user-attachments/assets/e7af4514-de85-4fcd-ac70-3f4b8efd63a0)

Розмір: <img width="84" height="39" alt="image" src="https://github.com/user-attachments/assets/81cf5583-d66d-402d-9cbf-44da351c1a0e" />

**2.Скріншот**

<img width="1052" height="434" alt="Снимок экрана 2025-11-25 094925" src="https://github.com/user-attachments/assets/cbf8e78b-c7d2-4e69-83da-93d977a6b0ef" />

Розмір: <img width="61" height="40" alt="image" src="https://github.com/user-attachments/assets/6ca5d4e8-84bc-485a-817f-70f919b48dce" />

**3.Графічне зображення з текстом**

![1643633201_2-papik-pro-p-iphone-logotip-2](https://github.com/user-attachments/assets/bd13ef02-af0f-47d1-bad8-e90a428829c5)

Розмір: <img width="57" height="24" alt="image" src="https://github.com/user-attachments/assets/3b32aa68-c39e-461b-bedc-09b631da75b4" />

#### **2. Стиснення без втрати якості (lossless)**
- Завантажте кожне зображення в Squoosh
- Використайте формати PNG (lossless) та WebP (lossless).
- Зафіксуйте зміни у вазі файлу після кожного перетворення.
- Переконайтеся, що якість зображення залишилася незмінною

**1.Фото**

<img width="1001" height="728" alt="image" src="https://github.com/user-attachments/assets/60c2ea27-1029-48d9-8536-27f30b5345c8" />

Фотографія у форматі PNG стала значно більше важити 498 Кб замість 55 КБ 

<img width="1087" height="785" alt="image" src="https://github.com/user-attachments/assets/07ea2be8-939a-414b-a0d3-5051ba1f4e76" />

У форматі WebP наша фотографія також стала значно важчою із 55 КБ вона стала 214 КБ

**2.Скріншот**

<img width="1050" height="737" alt="image" src="https://github.com/user-attachments/assets/3c1c94c0-31bc-4ee8-b142-1aeeb58d4a10" />

Розмір скріншота з 256 КБ збільшився аж до 343 КБ в форматі PNG

<img width="1061" height="739" alt="image" src="https://github.com/user-attachments/assets/fd66668f-6985-4814-b76d-8ee184ddbd70" />

Після використання формату WebP забимо що в цьому випадку навпаки скріншот із 262 КБ став 153 КБ

**3.Графічне зображення з текстом**

<img width="1058" height="743" alt="image" src="https://github.com/user-attachments/assets/4e991136-3416-4fb0-973f-74ea65c97bf9" />

Розмір графічного зображженя з текстом з 46 КБ виросло до 134 КБ в форматі PNG

<img width="1077" height="734" alt="image" src="https://github.com/user-attachments/assets/d5bd46d5-0852-48b6-8af4-9cca5e6181fb" />

Розмір зображженя в форматі WebP стало 37.5 КБ замість 46 КБ стокового зображеня

#### **3. Стиснення з втратою якості (lossy)**

- Використайте формати MozJPEG, WebP (lossy) та AVIF.
- Виконайте стиснення на рівнях якості 100%, 75% та 50%.
- Зафіксуйте зміни розміру файлу.
- Визначте мінімальний рівень якості, при якому зображення залишається прийнятним.

**1.Фото**

*Рівень якості 100%:*
MozJPEG

<img width="1003" height="709" alt="image" src="https://github.com/user-attachments/assets/d50f24f7-fa1b-4e8f-b6e6-c3dacaa43ed6" />

Вага фото з 55 Кб виросла до 119 КБ

*Рівень якості 75%:*
MozJPEG

<img width="1701" height="924" alt="Снимок экрана 2025-11-28 100649" src="https://github.com/user-attachments/assets/ffb6cc35-53ca-486d-8608-8dc0398ee6f7" />

Зображення стало значно легшим з 55 КБ до 29 КБ

*Рівень якості 50%:*
MozJPEG

<img width="978" height="648" alt="image" src="https://github.com/user-attachments/assets/1a246be1-9af9-4864-8e49-bdc80c4f5c9f" />

Вага фото стала 17 КБ замість 55 КБ

*Рівень якості 100%:*
WebP

<img width="981" height="552" alt="image" src="https://github.com/user-attachments/assets/191de3e6-534f-49b4-bb5f-d24efc75c598" />

Вага фото з 55 Кб виросла до 214 КБ

*Рівень якості 75%:*
WebP

<img width="971" height="563" alt="image" src="https://github.com/user-attachments/assets/df13504e-f6ab-408d-88d5-2b6cb6114f2a" />

Вага фото з 55 Кб зменшилася до 22.4 КБ

*Рівень якості 50%:*
WebP

<img width="995" height="539" alt="image" src="https://github.com/user-attachments/assets/4c47fec9-ae6a-4d23-a153-60547b49397b" />

Вага фото з 55 Кб зменшилася до 15 КБ

*Рівень якості 100%:*
AVIF

<img width="936" height="472" alt="image" src="https://github.com/user-attachments/assets/d12097ef-3eda-4bcd-b3a0-82e2da15cfe0" />

Вага фото з 55 Кб виросла до 77.5 КБ

*Рівень якості 75%:*
AVIF

<img width="972" height="606" alt="image" src="https://github.com/user-attachments/assets/24a2c48a-cb35-435b-ae79-b06b1750d5b4" />

Зображення стало легшим з 55 КБ до 32 КБ

*Рівень якості 50%:*
AVIF

<img width="985" height="602" alt="image" src="https://github.com/user-attachments/assets/5517cc46-1a65-4dbe-af44-dffc31de8a0f" />

Вага фото стала 14 КБ замість 55 КБ

**2.Скріншот**

*Рівень якості 100%:*
MozJPEG

<img width="995" height="675" alt="image" src="https://github.com/user-attachments/assets/b411fff6-d50b-4a4b-bf42-0acdcd98eddc" />

Вага фото з 263 Кб зменшилася до 204 КБ

*Рівень якості 75%:*
MozJPEG

<img width="983" height="727" alt="image" src="https://github.com/user-attachments/assets/715a7f07-daac-4ac6-a498-165082e7651b" />

Вага фото з 263 Кб зменшилася до 32 КБ

*Рівень якості 50%:*
MozJPEG

<img width="981" height="728" alt="image" src="https://github.com/user-attachments/assets/5c295675-0be6-4f3c-b52b-150107918acc" />

Вага фото з 263 Кб зменшилася до 29 КБ(фото втратило значну якість)

*Рівень якості 100%:*
WebP

<img width="973" height="598" alt="image" src="https://github.com/user-attachments/assets/f24ba08d-d87e-42ea-8316-69828c93ffc2" />

Вага фото з 263 Кб зменшилася до 71 КБ

*Рівень якості 75%:*
WebP

<img width="990" height="527" alt="image" src="https://github.com/user-attachments/assets/2908743c-ebe5-4ba2-b26e-5f530ac1132b" />

Вага фото з 263 Кб зменшилася до 24 КБ

*Рівень якості 50%:*
WebP

<img width="966" height="566" alt="image" src="https://github.com/user-attachments/assets/58a1e9f8-7599-4032-8aa6-e533511af1ed" />

Вага фото з 263 Кб зменшилася до 19 КБ

*Рівень якості 100%:*
AVIF

<img width="972" height="615" alt="image" src="https://github.com/user-attachments/assets/c5245471-d4cd-45ce-85bc-941c3c90894e" />

Вага фото з 55 Кб виросла до 75 КБ

*Рівень якості 75%:*
AVIF

<img width="975" height="566" alt="image" src="https://github.com/user-attachments/assets/a1cf2134-72f3-47ee-80b6-9f950bee55fe" />

Зображення стало легшим з 263 КБ до 25 КБ

*Рівень якості 50%:*
AVIF

<img width="981" height="515" alt="image" src="https://github.com/user-attachments/assets/52341f92-e1c3-4b4b-9209-f674187c74ea" />

Вага фото стала 263 КБ замість 15 КБ

**3.Графічне зображення з текстом**

*Рівень якості 100%:*
MozJPEG

<img width="976" height="630" alt="image" src="https://github.com/user-attachments/assets/d672977b-e59e-4fb7-8ec3-38a8212f76f1" />

Вага фото з 46 Кб зменшилася до 43 КБ

*Рівень якості 75%:*
MozJPEG

<img width="1020" height="693" alt="image" src="https://github.com/user-attachments/assets/0acc4098-848e-4d32-a9e0-7740ec3ff396" />

Вага фото з 46 Кб зменшилася до 17 КБ

*Рівень якості 50%:*
MozJPEG

<img width="1009" height="657" alt="image" src="https://github.com/user-attachments/assets/49c45ad8-eb0c-40f2-9215-ab994e345277" />

Вага фото з 46 Кб зменшилася до 14 КБ

*Рівень якості 100%:*
WebP

<img width="979" height="594" alt="image" src="https://github.com/user-attachments/assets/79836cf6-b771-4399-a6b8-a69a59ae60dc" />

Вага фото з 46 Кб зменшилася до 23.5 КБ

*Рівень якості 75%:*
WebP

<img width="986" height="724" alt="image" src="https://github.com/user-attachments/assets/d6079af0-5f26-46c7-8a99-1653f4ecd88b" />

Вага фото з 46 Кб зменшилася до 9.4 КБ

*Рівень якості 50%:*
WebP

<img width="976" height="576" alt="image" src="https://github.com/user-attachments/assets/24f7fcbb-7f7c-4383-badd-4012fadf9f48" />

Вага фото з 46 Кб зменшилася до 8 КБ

*Рівень якості 100%:*
AVIF

<img width="1024" height="682" alt="image" src="https://github.com/user-attachments/assets/b991cd6c-3f08-4f57-bf38-1e764c5ee5fc" />

Вага фото з 46 Кб зменшилася до 22.5 КБ

*Рівень якості 75%:*
AVIF

<img width="1029" height="647" alt="image" src="https://github.com/user-attachments/assets/239f8274-33e7-47ed-8305-bcb3ad3953de" />

Зображення стало легшим з 46 КБ до 7.5 КБ

*Рівень якості 50%:*
AVIF

<img width="1004" height="692" alt="image" src="https://github.com/user-attachments/assets/420474c1-d6c7-4efa-95e6-795871629726" />

Вага фото стала 46 КБ замість 4 КБ

#### **4. Оптимізація розміру відповідно до цільового використання**
- Зменшіть розмір зображень відповідно до їхнього застосування:
- Для вебу: максимальна ширина 1200 px.
- Для мобільних пристроїв: максимальна ширина 600 px.
- Для Retina-дисплеїв: створіть 2x або 3x версію зображення.
- Зафіксуйте зміни у вазі файлу після кожного етапу.

**1.Фото**

*Формат 1200 для веб:*

<img width="984" height="863" alt="image" src="https://github.com/user-attachments/assets/f68b7ff7-94aa-4001-a984-0c4d30d0dc8e" />

Вага фото з 55 Кб зменшилася до 29 КБ

*Формат 600 для мобільних:*

<img width="1031" height="837" alt="image" src="https://github.com/user-attachments/assets/6affe8ea-84df-4c6e-b8a0-64f5c33bd83c" />

Вага фото з 55 Кб зменшилася до 26.3 КБ

*Формат для Retina 2x(2400):*

<img width="1040" height="752" alt="image" src="https://github.com/user-attachments/assets/e4f310ab-5847-488a-856e-f42420de3411" />

Вага фото стала 192 КБ замість 55 КБ

**2.Скріншот**

*Формат 1200 для веб:*

<img width="1041" height="851" alt="image" src="https://github.com/user-attachments/assets/8a445186-d43f-4672-9b88-ac04db09e080" />


Вага фото з 263 Кб зменшилася до 42.4 КБ

*Формат 600 для мобільних:*

<img width="970" height="829" alt="image" src="https://github.com/user-attachments/assets/99963279-2773-4e0c-9ec3-566795783cd0" />

Вага фото з 263 Кб зменшилася до 16 КБ(втратилась якість картинки)


*Формат для Retina 2x(2400):*

<img width="1060" height="832" alt="image" src="https://github.com/user-attachments/assets/e28148af-4b6f-44aa-8faa-47ee474ad717" />

Вага фото з 263 Кб зменшилася до 102 КБ

**3.Графічне зображення з текстом**

*Формат 1200 для веб:*
<img width="987" height="794" alt="image" src="https://github.com/user-attachments/assets/7a4795f8-3b9f-4879-b5ea-1f7631b733e1" />

Вага фото з 46 Кб зменшилася до 12 КБ

*Формат 600 для мобільних:*

<img width="1027" height="833" alt="image" src="https://github.com/user-attachments/assets/e538c145-fe08-404c-853a-a146d5da90e5" />

Вага фото з 46 Кб зменшилася до 5.5 КБ(значно гірша якість)

*Формат для Retina 2x(2400):*

<img width="993" height="847" alt="image" src="https://github.com/user-attachments/assets/ae803dc1-af6f-4a37-8766-4ca0f1acc1c6" />

Вага фото стала 46 КБ замість 31 КБ

#### **5.  Візуальний аналіз та висновки**

