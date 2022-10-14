Порядок установки:
1. обновляем пакеты
sudo apt update && sudo apt upgrade -y
2. скачиваем репозиторий:
git clone https://github.com/tarabukinivan/haqq_bot.git
3. Устанавливаем nodejs и npm
curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash - && \
sudo apt-get install nodejs -y && \
echo -e "\nnodejs > $(node --version).\nnpm  >>> v$(npm --version).\n"
4. переходим в папку проекта и устанавливаем необходимые модули
cd /$USER/haqq_bot
npm i
5. создаем файл .env и вводим необходимые данные для работы бота в файл .env
nano env
[code]
BOT_TOKEN=TOKEN
VALOPER=valoper_address
CHATID=chat_id
INFOTIME=300
[/code]
