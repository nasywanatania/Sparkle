
import sys
import time

def jalanin_lirik():

    lirik = [
        ("Zutto nani ka wo… berani ka wo… sagashite iru....", 0.1),
        ("Iiyou to omottan da, omae ga sekai no doko ni idemo, ore ga kanarazu ichido ai ni ikutte...", 0.09),
        ("Omae wa… berani da…? bijih wa doushite koko ni kita ? aitsu ni, aitsu ni au jinak ni kita. Tasukeru jinak ni kita. Ini dia hoshikatta...", 0.09),
        ("Daijina hito, wasuretakunai hito, wasurecha dame na hito. Berani da, berani da, berani da, namae wa...", 0.09),
        ("Watashitachi wa aeba zettai, sugu ni wakaru...", 0.09),
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
