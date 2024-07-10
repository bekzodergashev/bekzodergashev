misollar = input("Sana kiriting: ").split(',')
oylar = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"]

for matn in misollar:
    matn = matn.strip()
    sana_va_vaqt = matn.split(' ')
    sana = sana_va_vaqt[0].split('.')
    vaqt = sana_va_vaqt[1].split(':')
   
    kun = int(sana[0])
    oy = oylar[int(sana[1]) - 1]
    yil = int(sana[2])
    soat = int(vaqt[0])
    daqiqa = int(vaqt[1])
    inson_formati = f"{kun} {oy} {yil}-yil {soat} soat {daqiqa} minut"
    
    print(f"Komp formati: {matn} -> Inson formati: {inson_formati}
