# Vishwa CTF 2021
## Invalid
### Informasi Soal
| Kategori | Poin |
|----------|------|
| Networking | 392 |

## Deskripsi
![image](screenshot/soalInvalid.png)\
In the previous challenge's file, what was the ip of the person who entered the wrong credentials?

## Penyelesaian Soal
Diberikan sebuah *clue* untuk mencari *Flag* pada file question.pcapng dari Soal sebelumnya yaitu [Write up Commenting is the key](README.md) <br />
pada kali ini kami mencari alamat IP dari seseorang yang memasukan input dengan kesalahan password.<br />
1. Menggunakan *tools* *wireshark* pada Kali Linux
2. Kemudian masukan file dari soal [Comenting is the key](../CommentingistheKey/question.pcapng)
3. Lakukan *open file* seperti pada gambar berikut![image](screenshot/fileSoal.png)
4. Tuliskan pada *current filter* yaitu *frame contains password* yang mana akan memberi tahu kepada kita detail dari hal tersebut ![image](screenshot/flag.png)
5. Secara otomatis terdapat lah *Flag* nya.


## Flag
> vishwaCTF{212.242.33.35}
