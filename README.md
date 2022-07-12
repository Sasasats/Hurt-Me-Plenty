# Hurt-Me-Plenty

1. Создайте ветку storm и добавьте коммит в файл storm.txt:
Twenty ships with Norsemen braves
Riding the northern wind
1.1. git checkout -b storm
1.2. touch storm.txt
1.3. echo "Twenty ships with Norsemen braves
> Riding the northern wind" > storm.txt
1.4. git add storm.txt
1.5. git commit -m "added storm.txt file with 2 lines"

2. Добавьте еще 2 строки в storm.txt и сделайте еще один коммит:
They left their shores at early dawn
As a red sun was rising in the east
2.1. vim storm.txt
2.2. git add storm.txt
2.3. git commit -m "added two more lines to the storm.txt file"

3. Вернитесь в main и создайте файл pursuit.txt с текстом ниже:
The warming sun returns again
And melts away the snow
The sea is freed from icy chains
Winter is letting go
Выполните коммит.
3.1. git checkout main
3.2. touch pursuit.txt
3.3. echo "The warming sun returns again
> And melts away the snow
> The sea is freed from icy chains
> Winter is letting go" > pursuit.txt
3.4. git add pursuit.txt
3.5. git commit -m "added pursuit.txt file with 4 lines"

4. Отметьте коммит тегом session1 и перейдите в ветку storm
4.1. git tag session1
4.2. git checkout storm

5. Сделайте rebase ветки storm так чтобы она содержала последний коммит из main.
5.1. git cherry-pick session1
