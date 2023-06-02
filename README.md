# DZ-18.12
Домашнее задание к модулю 18

Пргорамма, считывает из файла при своей загрузке данные и выводит их, записывает в файл состояния объектов классов User и Message (нужные данные указаны в программе),  и опять таки считывает и выводит их на консоль; в случае отсутствия файлов программа их создает (для каждого класса свой файл), а первоначально выводит пустую строку и текстовое предупреждение что данные отсутствуют.

class User {
    string _name;
    string _login;
    string _pass;
};
class Message {
    string _text;
    string _sender;
    string _receiver;
};

Эта часть задания: 

    Сделайте это таким образом, чтобы файлы были недоступным для других пользователей, то есть чтобы информацию из файлов прочитать или записать туда информацию мог бы только пользователь, который запускает программу. 

реализована с помощью system библиотеки cstdlib (stdlib.h   ), в которой прописана строка с раздачей прав chmod 600 (владельцу разрешена запись и чтение; остальным ничего) на создаваемые файлы.
