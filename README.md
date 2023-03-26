<h2 style="text-align:center; font-size:28px;">Kruskal Algoritması ile Minimum Birim Ağırlıklı Ağaç Oluşturma</h2>
<p style="text-align:justify; font-size:18px;">
Bu kod, Kruskal algoritmasını kullanarak ağırlıklı olmayan bir grafa minimum birim ağırlıklı ağaç (minimum spanning tree) oluşturmak için kullanılır. Algoritma, adım adım en küçük ağırlıklı kenarları seçer ve birleştirir. Birleştirme işlemi, hiyerarşik bir ağaç yapısı oluşturarak gerçekleştirilir.
</p>
<p style="text-align:justify; font-size:18px;">
Bu kodda, <code>Graph</code> sınıfı, graf veri yapısını temsil etmek için kullanılır. <code>kenar_ekle()</code> fonksiyonu, grafın kenarlarını eklemek için kullanılır. <code>kruskal_mst()</code> fonksiyonu, Kruskal algoritmasını uygular ve minimum birim ağırlıklı ağacı hesaplar.
</p>
<p style="text-align:justify; font-size:18px;">
Kodun sonunda, ağacın çizimi için <code>networkx</code> ve <code>matplotlib</code> kütüphaneleri kullanılmıştır. <code>minimum_spanning_tree()</code> fonksiyonu, ağacı oluşturmak için kullanılır ve <code>spring_layout()</code> fonksiyonu, düğümlerin konumlarını belirlemek için kullanılır. Sonuç olarak, ağacın çizimi <code>plt.show()</code> fonksiyonu ile görüntülenir.
</p>
<p style="text-align:justify; font-size:18px;">
Aşağıda, Kruskal algoritması ile oluşturulan minimum birim ağırlıklı ağacın görselleştirilmiş halini görebilirsiniz.
</p>
<div style="text-align:center">
<img src="https://user-images.githubusercontent.com/72278651/227801082-a599749c-3461-42fd-b6ab-9cf8f86bd3a5.png" width="400" />
</div>
<p style="text-align:justify; font-size:18px;">
Örnek kullanım:
</p>
<pre style="background-color:#f4f4f4; font-size:16px; padding:10px">
g = Graph()
g.kenar_ekle('A', 'B', 2)
g.kenar_ekle('A', 'C', 3)
g.kenar_ekle('B', 'C', 1)
g.kenar_ekle('B', 'D', 1)
g.kenar_ekle('C', 'D', 4)
g.kruskal_mst()
</pre>


