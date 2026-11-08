# Privacy Policy for Goal Tracker

**Last updated:** November 5, 2026

This Privacy Policy applies to the **Goal Tracker** mobile application ("the App"), developed as an offline-first personal productivity tool.

---

## 1. Summary (Privacy by Design)

- **100% Offline-First:** Goal Tracker does not require an account, registration, or internet connection to function.
- **No Data Collection:** We do not collect, transmit, store, sell, or share any personal information, usage analytics, or telemetry with external servers or third parties.
- **Your Data Stays on Your Device:** All your goals, habits, financial plans, streaks, reminders, and history are stored locally in an encrypted/isolated SQLite database on your device.

---

## 2. Information We Handle Locally

All data created or configured within the App is processed exclusively on your device:

1. **User-Generated Content:**
   - Goal titles, descriptions, target dates, monetary targets, habit categories, and completion logs.
   - Stored strictly in local app storage via SQLite.
2. **Security Credentials (PIN & Biometrics):**
   - If you enable the App Lock feature:
     - **PIN Code:** Salted and hashed locally on your device; never sent anywhere.
     - **Biometrics (Fingerprint / Face Unlock):** Handled entirely by the Android operating system's secure hardware enclave (`BiometricPrompt` / KeyStore). The App never sees, accesses, or stores your biometric raw data; it only receives a boolean confirmation from the OS.
3. **App Preferences & Settings:**
   - Selected language, visual theme, reminder preferences, and notification sound settings. Stored locally via Android `SharedPreferences`.

---

## 3. Device Permissions and Why We Need Them

Goal Tracker requests only the minimum permissions necessary for offline functionality:

- **Notifications (`android.permission.POST_NOTIFICATIONS`):**  
  Used solely to display scheduled local reminders for your goals and habits at times you explicitly choose. Notifications are generated and scheduled entirely on-device (`flutter_local_notifications`).
- **Run at Startup (`android.permission.RECEIVE_BOOT_COMPLETED`):**  
  Used to reschedule your active local reminders after your device restarts or reboots.
- **Biometric Hardware (`android.permission.USE_BIOMETRIC`):**  
  Used to unlock the App using your device's fingerprint or face unlock sensor if you choose to enable biometric security.

Goal Tracker **does not** request permissions for your location, contacts, microphone, camera, or device identifiers (IMEI/MAC).

---

## 4. Backups and Data Export

- **Manual Export:** You can export your data at any time into a standard JSON file.
- **Data Destination:** The backup file is saved directly to your device's local storage (e.g., Downloads folder).
- **Your Responsibility:** You maintain full ownership and control over the exported backup files. The App will never automatically upload your backups to any cloud service.

---

## 5. Third-Party Services and Analytics

- **No Third-Party SDKs:** The App contains **no** advertising networks (e.g., Google AdMob), **no** analytics trackers (e.g., Google Analytics, Firebase, Mixpanel), and **no** third-party crash reporters.
- **No Third-Party Sharing:** Since no data is collected, no data is sold, rented, or shared with third parties.

---

## 6. Children's Privacy

Goal Tracker is safe for users of all ages. We do not collect any personal information from children or adults alike.

---

## 7. Changes to This Privacy Policy

If we ever update this Privacy Policy (for example, if new offline features are added), the updated policy will be posted in the App's repository with a revised "Last updated" date.

---

## 8. Contact Us

If you have questions, feedback, or concerns regarding this Privacy Policy or the App, please open an issue on our GitHub repository:
- **GitHub Repository:** https://github.com/lostyheaven/goal_tracker
- **Developer:** lostyheaven

---

<br/>

# Політика конфіденційності для Goal Tracker

**Останнє оновлення:** 5 листопада 2026 р.

Ця Політика конфіденційності поширюється на мобільний додаток **Goal Tracker** («Додаток»), створений як повністю автономний інструмент особистої продуктивності за принципом offline-first.

---

## 1. Головне (Конфіденційність за замовчуванням)

- **100% Offline-First:** Додаток не вимагає реєстрації, створення облікового запису або підключення до Інтернету для роботи.
- **Жодного збору даних:** Ми не збираємо, не передаємо, не зберігаємо на зовнішніх серверах і не продаємо вашу особисту інформацію, дані аналітики або телеметрію третім особам.
- **Ваші дані належать лише вам:** Усі ваші цілі, звички, фінансові плани, серії виконання, нагадування та історія зберігаються виключно локально у захищеній базі даних SQLite на вашому пристрої.

---

## 2. Інформація, яка обробляється локально

Усі дані, створені в Додатку, обробляються виключно на вашому пристрої:

1. **Користувацький контент:**
   - Назви цілей, описи, дати дедлайнів, суми заощаджень, категорії звичок та відмітки виконання.
   - Зберігаються суто в локальному сховищі додатка через SQLite.
2. **Дані безпеки (PIN-код та біометрія):**
   - Якщо ви увімкнули блокування додатка:
     - **PIN-код:** Хешується із сіллю локально на пристрої та нікуди не передається.
     - **Біометрія (відбиток пальця / розпізнавання обличчя):** Обробляється безпосередньо операційною системою Android (`BiometricPrompt` / апаратний анклав безпеки). Додаток не має доступу до біометричних даних і отримує від системи лише відповідь «успішно/неуспішно».
3. **Налаштування додатка:**
   - Обрана мова, візуальна тема, налаштування сповіщень. Зберігаються локально через `SharedPreferences`.

---

## 3. Дозволи додатку та навіщо вони потрібні

Goal Tracker запитує лише мінімально необхідні дозволи:

- **Сповіщення (`android.permission.POST_NOTIFICATIONS`):**  
  Використовується виключно для показу локальних нагадувань про ваші цілі та звички у встановлений вами час. Нагадування створюються повністю локально на пристрої (`flutter_local_notifications`).
- **Автозапуск після перезавантаження (`android.permission.RECEIVE_BOOT_COMPLETED`):**  
  Необхідний для відновлення розкладу локальних нагадувань після перезапуску телефона.
- **Використання біометрії (`android.permission.USE_BIOMETRIC`):**  
  Використовується для розблокування додатка за відбитком пальця, якщо ви активували цей захист у налаштуваннях.

Додаток **не запитує** дозволів на доступ до геолокації, контактів, мікрофона, камери чи унікальних ідентифікаторів пристрою.

---

## 4. Резервне копіювання та експорт даних

- **Ручний експорт:** Ви можете в будь-який момент експортувати свої дані у стандартний файл JSON.
- **Збереження файлу:** Резервна копія зберігається безпосередньо у внутрішню пам'ять вашого телефона (наприклад, у папку «Завантаження»).
- **Контроль:** Додаток ніколи не відправляє ваші резервні копії на сторонні хмарні сервіси без вашої особистої дії через системний діалог «Поділитися».

---

## 5. Сторонні сервіси та реклама

- **Ніяких сторонніх трекерів:** У додатку **немає** реклами, рекламних мереж, систем аналітики (Google Analytics, Firebase, Facebook SDK) та збирачів помилок.
- **Ніякої передачі інформації:** Оскільки додаток не збирає дані, ніяка інформація не продається і не передається третім сторонам.

---

## 6. Зворотний зв'язок та контакти

Якщо у вас виникли запитання щодо Політики конфіденційності або роботи додатку:
- **GitHub репозиторій:** https://github.com/lostyheaven/goal_tracker
- **Розробник:** lostyheaven
