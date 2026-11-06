import sys
import time


def jalanin_lirik():
    # Ubah lirik lagu dan delay hurufnya sesuai yang kalian mau
    lirik = [
        ("Temanku semua pada jahat tante...", 0.1),
        ("Aku lagi susah mereka gak ada...", 0.09),
        ("Coba kalo lagi jayaaa...", 0.09),
        ("Aku dipuja puja tante...", 0.09),
        ("Teman datang ketika lagi butuh saja...", 0.09),
        ("Coba kalau lagi susaahhhh...", 0.09),
        ("Mereka semua menghilaaaanggg🤣🤣🤭", 0.09),
    ]

    # Ubah delay dari setiap baris lagu (sesuaikan jumlah)
    delay = [0.3, 0.2, 0.3, 0.4, 0.6, 0.3, 0.3]
    # Ubah judul lagu
    print("\n== JJ - Temanku semwa pada jahat tante ==")
    for i, (baris_lagu, delay_karakter) in enumerate(lirik):
        for karakter in baris_lagu:
            print(karakter, end='')
            sys.stdout.flush()
            time.sleep(delay_karakter)
        time.sleep(delay[i])
        print('')
    # Ganti nama pembuat
    print("// Code by nasywa hafsah")


jalanin_lirik()
