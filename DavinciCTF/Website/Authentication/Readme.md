# Davinci CTF

## Authentication

## Informasi Soal
| Kategori | Poin |
| -------- | ---- |
| Website | 10 |

### Deskripsi
> Can you find a way to authenticate as admin?
>
>http://challs.dvc.tf:1337/ 
## Cara Penyelesaian
Terdapat sebuah link website, yang mana bila diklik akan menampilkan sebuah halaman login. Dari judul soal terdapat petunjuk authentication, dari petunjuk tersebut dapat ditarik kesimpulan bahwa website rentan pada authenticationnya. Maka selanjutnya saya mencoba untuk memasukkan payload Sql Injection Login.
```
' or 1=1 --
```
Sehingga menjadi seperti berikut:

![image](Images/2_injection.PNG)

Detail Login :
```
Username = ' or 1=1 --
Password = ' or 1=1 --
```
Dan ternyata berhasil untuk masuk ke sistem artinya website tersebut rentan terhadap SQL Injection Login. Selanjutnya saya membuka inpect element, dan pada source codenya ditemukan flag dari soal.
![image](Images/3_inspect.PNG)
## Flag

> dvCTF{!th4t_w4s_34sy!}