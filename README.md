# Get next line
### 42 - Project #3

### From the PDF

You are now starting to understand that it will get tricky to read data from a file descriptor if you don’t know its size beforehand. What size should your buffer be? How many times do you need to read the file descriptor to retrieve the data ?

It is perfectly normal and natural that, as a programmer, you would want to read a “line” that ends with a line break from a file descriptor. For example each command that you type in your shell or each line read from a flat file.

Thanks to the project get_next_line, you will finally be able to write a function that will allow you to read a line ending with a newline character from a file descriptor. You’ll be able to add this function to your libft if you feel like it and most importantly, use it in all the future projects that will require it.

For the complete instructions, check out the [PDF].

### Usage

Since get_next_line() is a function, you can use it like this:

```c
char *line;

// To get a single line
get_next_line(fd, &line);
// Print the line
ft_putstr(line);
// Free after you're done using your line
free(&line);

// To read a whole file
while (get_next_line(fd, &line))
{
	// Print the line
	ft_putstr(line);
	// Free after you're done using your line
	free(&line);
}
```

[PDF]: https://github.com/erredavila/get_next_line/blob/master/get_next_line.en.pdf
