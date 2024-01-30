# Kodlar
def buyuk_herflerle_cap_et(soz):
    return soz.upper()

# Funksiyanı tətbiq etmək üçün nümunə list
sozler = ["salam", "dunya", "python"]

# map funksiyası ilə bütün sözləri böyük hərflərlə çap etmək
cap_edilmis_sozler = list(map(buyuk_herflerle_cap_et, sozler))

print(cap_edilmis_sozler)






def quvvet_yukselt(list):
    return [eded ** eded for eded in list]

# Funksiyanı tətbiq etmək üçün nümunə list
ededler = [2, 3, 4, 5]

# Ədədləri öz qüvvətinə yüksəltmək üçün list comprehension
quvvet_yukseltilmis_ededler = quvvet_yukselt(ededler)

print(quvvet_yukseltilmis_ededler)





def cut_eded_mi(eded):
    return eded % 2 == 0

def kvadrat_hesabla(eded):
    return eded ** 2

# Funksiyanı tətbiq etmək üçün nümunə list
ededler = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# filter və map funksiyalarını birgə istifadə etmək
cut_ededler = filter(cut_eded_mi, ededler)
kvadratlar = map(kvadrat_hesabla, cut_ededler)

# Nəticəni listə çevirmək
kvadratlar_list = list(kvadratlar)

print(kvadratlar_list)





# Funksiyanı tətbiq etmək üçün nümunə list
ededler = [-2, -1, 0, 1, 2, 3, 4, 5, 6]

# filter və lambda funksiyalarını istifadə etmək
musbet_ededler = list(filter(lambda x: x > 0, ededler))

print(musbet_ededler)
