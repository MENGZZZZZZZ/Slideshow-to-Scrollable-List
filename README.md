package com.example.slideshowapp

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity
import androidx.recyclerview.widget.LinearLayoutManager
import androidx.recyclerview.widget.RecyclerView

class MainActivity : AppCompatActivity() {

    private lateinit var recyclerView: RecyclerView

    private val imageList = listOf(
        ImageItem(R.drawable.hello, "Hello"),
        ImageItem(R.drawable.citylights, "City Lights"),
        ImageItem(R.drawable.desert, "Desert"),
        ImageItem(R.drawable.fireworks, "Fireworks"),
        ImageItem(R.drawable.forestopath, "Forest Path"),
        ImageItem(R.drawable.beachvibes, "Beach Vibes"),
        ImageItem(R.drawable.lakemirror, "Lake Mirror"),
        ImageItem(R.drawable.mountainroad, "Mountain Road"),
        ImageItem(R.drawable.rainystreet, "Rainy Street"),
        ImageItem(R.drawable.starrynight, "Starry Night"),
        ImageItem(R.drawable.sunsetview, "Sunset View"),
        ImageItem(R.drawable.thankyouforwatching, "Thanks for Watching")
    )


    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        recyclerView = findViewById(R.id.recyclerView)
        recyclerView.layoutManager = LinearLayoutManager(this)
        recyclerView.adapter = ImageAdapter(imageList)
    }
}

---------------------------------

ImageItem.kt:  

package com.example.slideshowapp

data class ImageItem(
    val imageResId: Int,
    val caption: String
)


![f83104f5d112bd411844d97cec811e5](https://github.com/user-attachments/assets/e5849d81-865c-4cfe-ae57-9894998e610a)
![449661626079ff1e9ddd6f7ca404f18](https://github.com/user-attachments/assets/70af728c-d136-4a8e-916d-2ced59887de4)
![19d6f5e4553463b6cca7f36754f1675](https://github.com/user-attachments/assets/08c51f60-a27d-42a9-b78d-b9af74898722)
![f4b35a9d2aed98f91c73ac23902e8d0](https://github.com/user-attachments/assets/ff422443-3c2f-405c-9cae-690ac44aea4f)
![a07c462304c86fe9942d839e486736f](https://github.com/user-attachments/assets/a77c55a2-565c-431d-8c40-80a2547ecc9c)
![a5145c0da8d679134e70d609f523dee](https://github.com/user-attachments/assets/ed7bcf3e-ccf6-4f6c-8f64-b2ccdc538ce0)





