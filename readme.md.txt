# Простой калькулятор на Python

def add(x, y):
    """Функция для сложения двух чисел."""
    return x + y

def subtract(x, y):
    """Функция для вычитания одного числа из другого."""
    return x - y

def multiply(x, y):
    """Функция для умножения двух чисел."""
    return x * y

def divide(x, y):
    """Функция для деления одного числа на другое."""
    if y == 0:
        return "Ошибка: деление на ноль!"
    return x / y

print("Выберите операцию:")
print("1. Сложение")
print("2. Вычитание")
print("3. Умножение")
print("4. Деление")

choice = input("Введите номер операции (1/2/3/4): ")

num1 = float(input("Введите первое число: "))
num2 = float(input("Введите второе число: "))

if choice == '1':
    print("Результат сложения:", add(num1, num2))
elif choice == '2':
    print("Результат вычитания:", subtract(num1, num2))
elif choice == '3':
    print("Результат умножения:", multiply(num1, num2))
elif choice == '4':
    print("Результат деления:", divide(num1, num2))
else:
    print("Неправильный ввод")
