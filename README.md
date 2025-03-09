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
