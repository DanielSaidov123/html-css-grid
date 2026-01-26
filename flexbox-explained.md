
# 📦 Flexbox – סיכום מוסבר (שורה־שורה)

המדריך הזה מסביר **כל פקודה ב־Flexbox**, מה היא עושה ובאיזה מצב משתמשים בה.

---

## הפעלת Flex

```css
display: flex;
```
הופך את האלמנט ל־Flex Container.  
מרגע זה כל הילדים שלו נשלטים ע"י Flexbox ומסתדרים אוטומטית.

---

## כיוון הסידור – flex-direction

```css
flex-direction: row;
```
מסדר את הילדים **בשורה אופקית** (משמאל לימין).  
זו ברירת המחדל.

```css
flex-direction: row-reverse;
```
כמו `row` אבל הסדר הפוך (מימין לשמאל).

```css
flex-direction: column;
```
מסדר את הילדים **בעמודה אנכית** (מלמעלה למטה).

```css
flex-direction: column-reverse;
```
עמודה הפוכה (מלמטה למעלה).

---

## יישור על הציר הראשי – justify-content

```css
justify-content: flex-start;
```
האלמנטים נדבקים להתחלה של הציר הראשי.

```css
justify-content: center;
```
ממרכז את האלמנטים על הציר הראשי.

```css
justify-content: flex-end;
```
מצמיד את האלמנטים לסוף הציר הראשי.

```css
justify-content: space-between;
```
רווח שווה **בין** האלמנטים (בלי רווח בקצוות).

```css
justify-content: space-around;
```
רווח מסביב לכל אלמנט (קצוות קטנים יותר).

```css
justify-content: space-evenly;
```
רווח שווה לחלוטין גם בין האלמנטים וגם בקצוות.

---

## יישור על הציר המשני – align-items

```css
align-items: stretch;
```
ברירת מחדל – האלמנטים נמתחים לגובה/רוחב של הקונטיינר.

```css
align-items: center;
```
ממרכז את האלמנטים על הציר המשני.

```css
align-items: flex-start;
```
מצמיד להתחלה של הציר המשני.

```css
align-items: flex-end;
```
מצמיד לסוף של הציר המשני.

```css
align-items: baseline;
```
מיישר לפי קו הטקסט (שימושי לטקסטים בגבהים שונים).

---

## שבירת שורות – flex-wrap

```css
flex-wrap: nowrap;
```
כל האלמנטים נשארים בשורה אחת (ברירת מחדל).

```css
flex-wrap: wrap;
```
כשאין מקום – האלמנטים יורדים שורה.

```css
flex-wrap: wrap-reverse;
```
כמו wrap אבל הסדר האנכי הפוך.

---

## קיצור דרך – flex-flow

```css
flex-flow: row wrap;
```
קיצור ל־  
`flex-direction: row;`  
`flex-wrap: wrap;`

---

# פקודות על הילדים (Flex Items)

## שליטה בגודל – flex

```css
flex: 1;
```
האלמנט יתפרס וימלא מקום שווה ביחס לאחים שלו.

```css
flex: grow shrink basis;
```
פירוק מלא של הפקודה:

- **grow** – כמה האלמנט יגדל
- **shrink** – כמה הוא יקטן
- **basis** – הגודל ההתחלתי

```css
flex: 1 0 200px;
```
האלמנט:
- יכול לגדול
- לא יקטן
- מתחיל מרוחב 200px

---

## יישור ילד ספציפי – align-self

```css
align-self: center;
```
ממרכז רק את האלמנט הזה.

```css
align-self: flex-end;
```
מצמיד רק את האלמנט הזה לסוף הציר המשני.

---

## שינוי סדר – order

```css
order: -1;
```
האלמנט יופיע ראשון.

```css
order: 1;
```
האלמנט יופיע אחרי אלמנטים עם order נמוך יותר.

---

## סיכום קצר
- `display: flex` – מפעיל Flexbox  
- `flex-direction` – קובע כיוון  
- `justify-content` – יישור על הציר הראשי  
- `align-items` – יישור על הציר המשני  
- `flex-wrap` – שבירת שורות  
- `flex` – שליטה בגודל האלמנט  
- `order` – שינוי סדר  

Flexbox = הדרך הכי נוחה, ברורה ומודרנית לסידור אלמנטים ב־CSS.
