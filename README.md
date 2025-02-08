import random
# Sambutan awal permainan
print('=============Selamat datang di permainan ini!!!===============')
print("Selamat datang di permainan Russian Roulette")
print("Jika angka yang kamu sebut betul, kamu akan ditembak!!")    
print('================ATURAN PERMAINAN==============================')

# Meminta input umur dari pemain
umur = int(input("Masukkan umur anda: "))

# Semak kelayakan umur
if umur >= 18:
    print('APAKAH ANGKANYAAA:!!!!!!!!!!!!!!')

    # Menjana nombor rawak antara 1 dan 4
    angka_terpilih = random.randrange(1, 5)

    
    teka = int(input("Masukkan angka antara 1 hingga 5: "))

    # Semak jika tebakan betul atau salah
    if teka == angka_terpilih:
        print("bingo! Kamu akan ditembak!")
    else:
        print("Selamat! Kamu tidak ditembak.")
else:
    print("Maaf, kamu belum cukup umur untuk bermain permainan ini.")
