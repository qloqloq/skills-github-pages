---
title: "Could not initialize proxy - no Session"
date: 2023-10-14
---
 ### Problem
 org.hibernate.LazyInitializationException: failed to lazily initialize a collection of role: com.example.vocabulary.model.Lesson.words: could not initialize proxy - no Session

### Solution
Added 	```@Transactional(readOnly = true)``` on the method level.
