# StreamMatch: Personalized Streaming Recommendations

## 1. Most Important Software Qualities

| Quality           | Reason for Importance |
|-------------------|------------------------|
| **Usability**     | Users like Soban need a simple, intuitive way to get show recommendations. |
| **Performance**   | Users expect fast, near-instant responses. |
| **Scalability**   | Should handle growing numbers of users and potential features. |
| **Modifiability** | Easy to update recommendation logic or UI components. |
| **Availability**  | Users typically use the system during evenings and weekends, so uptime matters. |

---

## 2. Architecture Overview 

### Layers Used:
- **User Interface**
- **User Interface Management**
- **Configuration Services**
- **Application Services**
- **Shared Infrastructure Services**

---

## 3. Architecture Diagram (inspired by Figure 4.11)

```plaintext
+------------------------------+
|        User Interface        |
|------------------------------|
| Web Browser                  |
+------------------------------+

+---------------------------------------------+
|     User Interface Management               |
|---------------------------------------------|
| Recommendation UI | Search | Login          |
+---------------------------------------------+

+------------------------------------------------+
|           Configuration Services               |
|------------------------------------------------|
| Viewing Preferences | Genre Filters | History  |
+------------------------------------------------+

+------------------------------------------------------+
|             Application Services                     |
|------------------------------------------------------|
| Get Recommendations | Fetch Show Data | Save History |
+------------------------------------------------------+

+--------------------------------------------------------+
|              Shared Infrastructure Services            |
|--------------------------------------------------------|
| PostgreSQL | IMDB API | Auth (JWT/OAuth) |             |
+--------------------------------------------------------+


4. Technologies To Be Used

Database: We would go use an unstructured NOSQL database due to new shows always being added into streaming service pools 

Platform: Web brower as we feel that a mobile app would be too much of an overkill for a product such as this 

Server: We plan to use a cloud provider in order to host our product with the team leaning towards the industry leaders being AWS or GCP

