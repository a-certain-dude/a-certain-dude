class DeveloperProfile {
    val name = "Nkwantabisa Joseph"
    val title = "Junior Kotlin Android Developer"
    val email = "nkwantabisajoseph25@gmail.com"
    val phone = "+233 596 003 162"
    val quote = "Building apps that solve real-world problems — one repo at a time."

    object Summary {
        val description = "Transitioning from learning to building real-world mobile and web applications using Kotlin, Jetpack Compose, and XML."
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

        object Tools {
            val libraries = listOf(
                "Git", 
                "GitHub", 
                "JUnit", 
                "Gradle", 
                "Retrofit", 
                "Room Database", 
                "Coil", 
                "kotlinx.coroutines.test"
            )
        }
    }

    object Projects {
        val marsPhotosApp = Project(
            name = "MarsPhotos App",
            description = "Kotlin app using Retrofit and coroutines to fetch NASA Mars Rover photos",
            details = listOf(
                "Inventory CRUD app using Room Database",
                "Unit tested with runTest, fake API, and coroutine testing libraries",
                "Follows repository pattern with NetworkMarsPhotosRepository"
            )
        )

        data class Project(
            val name: String,
            val description: String,
            val details: List<String>
        )
    }
}
