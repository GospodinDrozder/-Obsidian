Шаблон для ежедневных записей
<%*
var day = moment().format("dddd"); // "среда"
var capitalizedDay = day.charAt(0).toUpperCase() + day.slice(1); // "Среда"
var fileName = moment().format("D MMMM");
await tp.file.rename(fileName);
// Тест Moment.js
var now = moment();          // Создаем объект с текущей датой/временем
var formatted = now.format("DD MMMM YYYYг. HH:mm"); // Форматируем в строку
tR += `**${capitalizedDay} ${formatted}**\n`; // Выводим результат
tR += "______";
%>
