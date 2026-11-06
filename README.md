
import sys
import time

def jalanin_lirik():

    lirik = [
        ("Temanku semua pada jahat tante...", 0.1),
        ("Aku lagi susah mereka gak ada...", 0.09),
        ("Coba kalo lagi jayaaa...", 0.09),
        ("Aku dipuja puja tante...", 0.09),
        ("Sudah terbiasa terjadi tante...", 0.09),
        ("Teman datang ketika lagi butuh saja...", 0.09),
        ("Coba kalau lagi susaahhhh...", 0.09),
        ("Mereka semua menghilaaaanggg🤣🤣🤭", 0.09),
    ]

    # Delay antarbaris (8 baris lirik)
    delay = [0.3, 0.2, 0.3, 0.4, 0.6, 0.3, 0.3, 1.0]

    print("\n== JJ - Temanku Semua Pada Jahat Tante ==\n")

    for i, (baris_lagu, delay_karakter) in enumerate(lirik):

        for karakter in baris_lagu:
            print(karakter, end='', flush=True)
            time.sleep(delay_karakter)

        time.sleep(delay[i])
        print()

    print("\n// Code by Nasywa Hafsah")


jalanin_lirik()
