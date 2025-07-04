object Marcus {
    val age: Int = 23
    val from: String = "Yosef Nkwantabisa, Ghana"
    val languages: List<String> = listOf("English", "Twi")
    val interests: List<String> = listOf("Mobile Development")
    val curiosity: String = "I'm a strong defender of android"
    
    override fun toString(): String {
        return """
        Marcus:
        age: $age
        from: $from
        languages: $languages
        interests: $interests
        curiosity: $curiosity
		"""
    }
}
