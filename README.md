<h1 align="center">Cygwin on Windows</h1>

## Установка по-умолчанию
![](/img/1.jpg)

![](/img/2.jpg)

![](/img/3.jpg)

![](/img/4.jpg)

![](/img/5.jpg)

![](/img/6.jpg)

![](/img/7.jpg)

![](/img/8.jpg)

Затем находим папку с установщиком, если у вас браузер `Chrome` жмем `Ctrl+J` и  `Показать в папке` под установщиком `Cygwin`

![](/img/9.jpg)

![](/img/10.jpg)

Запускаем терминал `cmd.exe` из  текущей папки, как в инструкции на картинке, когда откроется терминал вставляем команду

```
setup-x86_64.exe -q -P lynx,wget,tar,git,vim
```
для установки пакетов *lynx,wget,tar,git,vim*   
дожидаемся окончания установки

![](/img/11.jpg)

Запускаем с Рабочего Стола `Cygwin`

![](/img/12.jpg)

скачиваем *apt-cyg*
```
wget -P /bin/ rawgit.com/transcode-open/apt-cyg/master/apt-cyg
```
и делаем его исполняемым

```
chmod +x /bin/apt-cyg
```

Устанавливаем *zsh*

```
apt-cyg install zsh
```
на ярлыке запуска `Cygwin` правую кнопку мыши и вставляем в поле *Объект:*
```
C:\cygwin64\bin\mintty.exe -i /Cygwin-Terminal.ico /bin/zsh --login
```

![](/img/16.jpg)

## Устанавливаем  [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

```
git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
```




