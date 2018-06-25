# CryptoProJcpExample
Пример использования КриптоПро JCP для генерации ключей, сертификатов и подписи

CryptoProJcpExample - веб приложение, написанное на springboot.
Для проверки надо зайти на localhost:8084/
При успешной подписи вы увидите саму подпись в 16тиричном представлении.
Кроме того, в конце должно быть verify: true (Это означает что подпись прошла проверку)

Веб приложение сначала пытается прочитать сертификаты из хранилища на жестком диске. Если хранилища нет, оно его создает со сгенерированным приватным ключом(предложит понажимать enter в консоли при первом запуске) и соответствующим сертификатом от тестового УЦ.

При входе на localhost:8084/ приложение подписывает тестовую строку и возвращает результаты подписи.


Больше примеров смотрите в samples.jar, который идет в поставке JCP. Там же документация. 
