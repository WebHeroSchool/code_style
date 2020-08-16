# 1. Фигурные скобки #

Фигурные скобки пишутся в так называемом «египетском» стиле с открывающей скобкой на той же строке, что и соответствующее ключевое слово – не на новой строке

- Плохой код

😠 Никогда не разделяйте строки без фигурных скобок, можно ненароком сделать ошибку при добавлении строк:

`if (n < 0)
  alert(`Степень ${n} не поддерживается`);`

- Хороший код

`if (n < 0) {
  alert(`Степень ${n} не поддерживается`);
}`
