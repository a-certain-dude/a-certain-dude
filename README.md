class DeveloperProfile {
    val name = "👋 Nkwantabisa Joseph"
    val title = "🎓 Junior Kotlin Android Developer"
    val contactEmail = "📧 nkwantabisajoseph25@gmail.com"
    val quote = "\"Building apps that solve real-world problems — one repo at a time.\""

    object Summary {
        val bio = """
            I'm a junior developer transitioning from learning to building 
            real-world mobile and web apps using Kotlin, Jetpack Compose, and XML.
        """.trimIndent()
    }

    object Skills {
        val languages = listOf("Kotlin", "Python")

        object Mobile {
            val tools = listOf(
                "Android Studio",
                "Jetpack Compose",
                "Material Design",
                "XML UI",
                "ViewModel",
                "Coroutines"
            )
        }

        object DevTools {
            val libraries = listOf(
                "Retrofit",
                "Room Database",
                "Coil",
            )
        }
    }

    object Projects {
        val marsPhotos = Project(
            name = "🛰 MarsPhotos App",
            description = "Kotlin app that fetches NASA Mars Rover photos using Retrofit and Coroutines.",
            highlights = listOf(
                "Inventory CRUD using Room Database",
                "Repository pattern: NetworkMarsPhotosRepository"
            )
        )

        data class Project(
            val name: String,
            val description: String,
            val highlights: List<String>
        )
    }

    fun introduce() {
        println("$name — $title")
        println("Contact me at $contactEmail or $contactPhone")
        println(quote)
    }
}
