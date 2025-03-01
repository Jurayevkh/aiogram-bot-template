# Aiogram Bot Shabloni

Telegram botlarini Aiogram yordamida ishlab chiqish uchun oson shablon. Telegram botingizni qurayotganda
tartib bilan qurishingiz uchun va keyinchalik rivojlantirish, kengaytirishda qulay shablon.

## 📂 Loyihaning Tuzilishi

```
📦 aiogram-bot-template
├── 📂 handlers
│   ├── 📂 users
│   ├── 📂 channels
│   ├── 📂 groups
│   └── __init__.py
├── 📂 keyboards
│   ├── 📂 inline
│   ├── 📂 default
│   └── __init__.py
├── 📂 utils
│   ├── notify_admin.py
│   ├── set_commands.py
├── 📂 data
│   └── config.py
├── 📂 database
│   ├── models.py
├── filters
│   ├── admin.py
├── requests.py
├── app.py  # Asosiy bot fayli
├── requirements.txt  # Kutubxonalar
└── README.md 
```

## 🚀 Vazifalari

- `app.py` botning asosiy ishga tushuvchi fayli, qaysi mode'da parse qilish, bot ishga tushganda ishlashi kerak bo‘lgan funksiyalarni sozlash kabi sozlamalar.
- `.env.dist` faylida `.env` faylida qanday ma’lumotlar bo‘lishi kerakligi yozilgan.
- `data/config.py` fayli `.env`dan ma’lumotlarni olib kelish uchun.
- `keyboards/default`,`keyboards.inline` botdagi oddiy va xabar osti tugmalarini saqlaydi, ikkala turdagi tugmadan `exampleDefaultKeyboard.py` va `exampleInlineKeyboard.py`da misol ko‘rshingiz mumkin.
- `handlers` faylida foydalanuvchilar,kanallar va guruhlar uchun alohida-alohida papka mavjud va foydalanuvchilar uchun /start va /help buyruqlari uchun handlerlar misol sifatida yozib qo‘yilgan.
- `database` faylida `models.py` va `request.py` fayli mavjud, sqlalchemy ORM yordamida bazaga ulanib table yaratishingiz va unga so‘rovlar yuborishingiz mumkin.
- `utils` qo‘shimcha funksiyalar yozishingiz uchun. Adminlarni bot ishga tushganidan xabardor qilish uchun `notify_admins.py` va bot buyruqlarini ko‘rinadigan qilib sozlash uchun `set_commands.py` fayllarini misol qilib olishingiz mumkin.
- `filters` xabarlarni tekshirish uchun filterlar yozasiz, xabar admindan yoki yo‘qligini tekshirish uchun `admin.py` filteri mavjud, misol sifatida olishingiz mumkin.
- `states` faylida statelarni yozasiz, misol sifatida `exampleState.py` mavjud.

## 📜 O‘rnatish va Sozlash

### 1️⃣ Repozitoriyani klonlash

```bash
git clone https://github.com/Jurayevkh/aiogram-bot-template.git
cd aiogram-bot-template
```

### 2️⃣ Kutubxonalarni o‘rnatish

```bash
pip install -r requirements.txt
```

### 3️⃣ Konfiguratsiyani sozlash

`.env` faylini yaratib, bot tokeni hamda kerakli ma'lumotlarni qo'shish.

```
BOT_TOKEN = "your-telegram-bot-token"
ADMINS = 123456789
```

### 4️⃣ Botni ishga tushirish

```bash
python app.py
```


🚀 **Aiogram va Python yordamida yaratilgan**

---
