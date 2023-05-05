
1. Створіть обліковий запис GitHub

https://github.com/join?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home

2. Встановіть CHOCOLATEY:
- запустіть powershell від імені адміністратора
- виконайте команду:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

![](/images/screen-1.png)

3. Встановіть git на ваш комп'ютер за допомогою Chocolatey:
```
choco install git -y
```
Ви можете використовувати термінал git bash для роботи з git або будь-який термінал.

4. Налаштуйте свій git:
```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

5. Згенеруйте новий SSH ключ:
![](/images/screen-2.png)

6. Додайте ключ до облікового запису Github:
- зкопіюйте /c/Users/you/.ssh/id_ed25519.pub 
- перейдіть за посиланням https://github.com/settings/keys
- натисніть зелену кнопку

- Вставте зкопійований ключ та натисніть відповідну кнопку
![](/images/screen-3.png)

Більше інформації: https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

Тепер ви можете використовувати GitHub

1. Створіть новий репозиторій
Назва репозиторію має бути такою як ваш нікнейм
![](/images/screen-4.png)

Переконайтеся, що репозиторій публічний та проініціалізований з readme.md файлом

2. Заберіть копію репозиторію на локальний комп'ютер:
- зкопіюйте посилання
- запустіть команду для клонування репозиторію:
```
git clone
```

![](/images/screen-5.png)

3. Відкрийте README.md вашим улюбленим текстовим редактором. 

4. Напишіть про себе
- З чим хотіли б попрацювати;
- Чим захоплюєтесь;
- Додайте посилання на свої соціальні мережі та ресурси, які вважаєте необхідними або бажаними

5. Завантажте опис вашого профілю:

![](/images/screen-6.png)

```
git add .
git commit -m "Add your comment"
git push


## Висновок

Після проведення лабораторної роботи ми отримали знання про використання git та GitHub. Ми навчилися принципам роботи з репозиторіями та опанували необхідні дії для зміни, додавання або видалення файлів з них. Крім того, ми розглянули форматування тексту для файлу README.md.

