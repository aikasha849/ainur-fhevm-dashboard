 Ainur's FHEVM Dashboard
Айнур — разработчик, исследователь и сторонник технологий, сохраняющих приватность. Этот проект — моя адаптация шаблона fhevm-react-template от Zama, основанная на версии 0.7 протокола FHEVM. Он демонстрирует, как можно обрабатывать и взаимодействовать с зашифрованными данными прямо на блокчейне с помощью полностью гомоморфного шифрования, сохраняя контроль и конфиденциальность пользователя.

🚀 Возможности
🔐 Увеличение и уменьшение зашифрованного счётчика

🧠 Запрос расшифровки через Decryption Oracle

🦊 Интеграция с MetaMask и тестовой сетью Sepolia

🧬 Использование FHEVM v0.7 и единиц гомоморфной сложности (HCU)

🧭 Шаги установки и деплоя
Проект был установлен и настроен вручную следующим образом:

Клонирование фронтенда Клонировала ветку alexB/nextjs-react-v7 репозитория fhevm-react-template

Клонирование Hardhat-бэкенда Из корня проекта:
cd ./packages
git clone https://github.com/zama-ai/fhevm-hardhat-template.git

Установка зависимостей Hardhat
cd fhevm-hardhat-template
npm install

Настройка переменных среды
npx hardhat vars set MNEMONIC
npx hardhat vars set ETHERSCAN_API_KEY

Компиляция и локальное тестирование контрактов
npm run compile
npm run test

Деплой в тестовую сеть Sepolia
npx hardhat deploy --network sepolia

Проверка контракта на Etherscan
npx hardhat verify --network sepolia <CONTRACT_ADDRESS>

Тестирование в сети Sepolia
npx hardhat test --network sepolia

Установка зависимостей фронтенда в корне проекта
cd ..
npm install

Запуск интерфейса
cd packages/site
npm run dev

Открыла http://localhost:3000 в браузере

Подключение MetaMask к Sepolia 
Переключила MetaMask на сеть Sepolia и протестировала взаимодействие с контрактом

📁 Структура проекта
packages/site/fhevm: хуки для взаимодействия с FHEVM-контрактами

packages/site/hooks/useFHECounter.tsx: пример логики зашифрованного счётчика

packages/site/hooks/metamask: хуки для подключения MetaMask

📚 Полезные ресурсы
Документация Zama FHEVM (https://docs.zama.ai/)

Гайд по настройке Hardhat + MetaMask (https://docs.zama.ai/protocol/solidity-guides/development-guide/migration)

@zama-fhe/relayer-sdk на npm (https://www.npmjs.com/package/@zama-fhe/relayer-sdk)

👤 Автор и контакты
Айнур — разработчик, исследователь и энтузиаст приватных технологий.
 Создано с ❤️ от Ainur$ZAMA

📬 Email: jeneshka883@gmail.com

💬 Telegram: @AinurSolar

🐦 X (Twitter): @InurSolar91279

🌐 Farcaster: farcaster.xyz/ainur-zk1
