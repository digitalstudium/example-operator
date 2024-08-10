1. Что такое оператор

2. Зачем он нужен

3. Предусловия

3.1 Установить docker и kubectl 
3.2 Установить minikube и стартовать его
3.3 Установить golang
3.4 Установить operator-sdk

4. Создание оператора

4.1 mkdir example-operator && cd example-operator && git init
4.2 operator-sdk init --domain example.com --repo github.com/digitalstudium/example-operator 
4.3 operator-sdk create api --group apps --version v1alpha1 --kind Example --resource --controller # список групп можно посмотреть командой kubectl api-resources -o name
4.4 git config user.name "Digital Studium" && git config user.email example@example.com && git add . && git commit -m "Clean operator"
4.5 Добавить функцию создания деплоя и импортировать либы
4.6 Изменить функцию Reconcile
4.7 Добавить оператору права на Kubernetes + добавить владение деплойментом

5. Развёртывание

5.1 развёртывание оператора
5.2 развёртывание приложения

6. Удаление

6.1 удаление приложения
6.2 удаление CRD
6.3 удаление оператора

Успехов в освоении Kubernetes!
