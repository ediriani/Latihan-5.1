def cek_angka(a, b, c):
    """
    Fungsi ini memeriksa apakah tiga parameter memenuhi ketentuan:
    - Semua nilai berbeda.
    - Ada dua parameter yang jika dijumlahkan sama dengan parameter lainnya.
    """
    if a == b or a == c or b == c:
        return False  # Nilai tidak berbeda semua

    if a + b == c or a + c == b or b + c == a:
        return True  # Ada dua parameter yang jika dijumlahkan sama dengan parameter lainnya
    else:
        return False  # Tidak ada dua parameter yang jika dijumlahkan sama dengan parameter lainnya

# Contoh penggunaan
print(cek_angka(1, 2, 3))  # True (1+2=3)
print(cek_angka(1, 2, 4))  # False (tidak ada yang dijumlahkan sama)
print(cek_angka(1, 1, 3))  # False (nilai tidak berbeda semua)
