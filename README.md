# Form Data

- Helps with sending HTML forms.

- Can be created by calling `new FormData()`.

- Fetch API can accept FormData as a body.

- It is encoded and sent out with `Content-Type: multipart/form-data` in fetch.

- We can modify and get fields in FormData: append, set, delete, get, has, getAll...

- Two versions when appending: `formData.append(name, value)`, `formData.append(name, value, filename)`

- We can iterate over its fields using for..of loop.

- To send a blob, binary data, you would append it to the formData: `formData.append("image", imageBlob, "image.png")`.

- Set method removes fields with the same name, append doesn't.

- When sending form data using the second version with 3 arguments, the last argument is a filename, usually taken from the filesystem for `<input type="file">`
