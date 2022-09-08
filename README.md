# Principal-Component-Analysis
Principal Component Analysis - Temel Bileşenler Analizi
Temel bileşenler analizi için veri dosyası yolu ve bileşen parametrelerini belirlemeniz yeterlidir.
---------------------------------------------------------------------------------------------------

#Veri dosyası yolu için
df = pd.read_csv('/content/drive/MyDrive/Examples/PCA/2015_2019_lab_v1_values.csv')

#Parametre - 1 - Verinin %95'ini açıklayan bileşenler için
pca_get_components = PCA(n_components=0.95, random_state=2020)

#Parametre - 2 - 31 kolonlu verinin herbir kolonunun toplam veriye etkisini görmek için
pca_start = PCA(n_components=31, random_state=2020)

#Parametre -1 ve -2 den yararlanarak bileşenler grafiği çıkarılmıştır.

#Grafik, verilen dosya yoluna yazdırılmıştır
plt.savefig ('/content/drive/MyDrive/Examples/PCA/PCA_Analysis_plot.png', dpi=1600)


#Çıktı verisi, verilen dosya yoluna yazdırılmıştır
df_new.to_csv('/content/drive/MyDrive/Examples/PCA/PCA_Output_data.csv', index=False)
