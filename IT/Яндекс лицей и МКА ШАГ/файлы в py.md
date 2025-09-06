
#python
#IT
os:
	`os.getcwd()` - название текущей папки
	`os.chdir()` - change directory

	`os.acsess():` - проверка состояния файла
1) `F_OF` - существует?
2) `R_OK `- 
3) `W_OK` - 
    `os.listdir()` = ls - все файлы в директории
	`os.walk()` - пройтись и посмотреть рекурсивно все [[файл]] и [[каталог]]и
	`os.path()` - 
	`os.isfile()` - файл или директория

shutil:
	copy() - создаст директорию, если такой ещё нет
	rmtree() - удалить папку с содержимым
	get_archive_formats() - работа с архивами
		make_archive()

zipfile:
	`with ZipFile("archive") as myzip` работа с архивом не распаковывая
		`myzip.infolist`
	wright - записать файл в директорию
	 #Яндекс_лицей 
	