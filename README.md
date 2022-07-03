# How to MySQL docker server?

1. Download and install [Docker](https://docs.docker.com/get-started/).
2. Make sure to switch to directory `mysql-docker-server`. The root directory 
of this repository may be occupied for other purposes in the future.
3. Run `docker compose up -d`

Yeah, that's all. Simple, isn't it?

If there were installation problems occured, contact me. I'm too lazy to 
write a documentation about that. Or maybe, you should search on Google first.

## Probable FAQs

Nobody has asked me yet, so I guess my own set of Q&A's.

1. **How to open Phpmyadmin?**<br>Browse `http://localhost:8080` and there you
go.

2. **Do I have to import the `company_elmasri.sql` file?**<br>No. We did it 
already in the `docker-compose.yml` file. You may need to take a look to learn 
about it.

3. **How to open Jupyter Lab?**<br>Browse `http://localhost:8888/?token=docker`.
Note that `?token=docker` is important here. Or you can input `docker` if you 
miss that part in the URL.

4. **Where does the practice notebook located?**<br>In Jupyter Lab, on the left 
pane, you'll see the only directory. Yes, that's where it's located.

5. **How can I connect to MySQL using Jupyter Lab?**<br>Read the practice 
notebook.

