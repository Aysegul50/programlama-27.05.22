# programlama-03.06.22

ABC=open("A.txt","w",encoding="utf-8")
OSayi=int(input("Öğrenci sayısını giriniz:"))

for i in range(OSayi):
    Vize=random.randint(0,100)
    Final=random.randint(0,100)
    Ort=int(Vize+Final/2)
    
    if(Ort>=50):
       Durum="GEÇTİ"
    else:
       Durum="KALDI"
    
    ABC.write(str(Vize)+" "+str(Final)+" "+str(Ort)+" "+Durum+"\n")
    
ABC.close()  
ABC=open("A.txt","r",encoding="utf-8")
print(ABC.read()) 
Veri=ABC.read()
ABC.close()
print(********************************)
print(Veri)

