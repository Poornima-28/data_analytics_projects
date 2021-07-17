
Project Description
Due to the global pandemic, more people were at home and reading books. This attracted the attention of startups that rushed to develop new apps for book lovers. The given database of one of the service competing in market consists data on books , publishers etc., This information must be used to generate a value proposition for a new product

Data Description:

books:
- book_id
- author_id
- title
- num_pages — number of pages
- publication_date
- publisher_id

authors:
- author_id
- author

publishers:
- publisher_id
- publisher

ratings:
- rating_id
- book_id
- username — the name of the user who rated the book
- rating

reviews:
- review_id
- book_id
- username — the name of the user who reviewed the book
- text — the text of the review
