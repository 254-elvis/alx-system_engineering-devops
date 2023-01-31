Project Description.
Learn about regular expressions and building them using Oniguruma library which uses Ruby by default.

Because the focus of this exercise is to play with regular expressions (regex), here is the Ruby code that you should use, just replace the regexp part, meaning the code in between the //:

sylvain@ubuntu$ cat example.rb
#!/usr/bin/env ruby
puts ARGV[0].scan(/127.0.0.[0-9]/).join
sylvain@ubuntu$
sylvain@ubuntu$ ./example.rb 127.0.0.2
127.0.0.2
sylvain@ubuntu$ ./example.rb 127.0.0.1
127.0.0.1
sylvain@ubuntu$ ./example.rb 127.0.0.a
0. Simply matching School - The regular expression must match School. - 0-simply_match_school.rb.
1. Repetition Token #0 - The regular expression must match the given cases. - 1-repetition_token_0.rb.
2. Repetition Token #1 - The regular expression must match the given cases. - 2-repetition_token_1.rb.
3. Repetition Token #2 - The regular expression must match the given cases. - 3-repetition_token_2.rb.
4. Repetition Token #3 - The regular expression must match the given cases. - 4-repetition_token_3.rb.

