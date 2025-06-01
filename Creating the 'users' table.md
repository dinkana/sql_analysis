# Создание таблицы 'users'

```sql
-- Optional: Drop the table if it already exists
DROP TABLE IF EXISTS users;

-- Create the users table
CREATE TABLE users(
    id INTEGER NOT NULL PRIMARY KEY,
    u_name VARCHAR(127) NOT NULL,
    email VARCHAR(127) NOT NULL,
    email_verified_at DATE NOT NULL,
    u_password VARCHAR(25) NOT NULL,
    phone_number VARCHAR(20)
);

-- Insert sample data
INSERT INTO users(id, u_name, email, email_verified_at, u_password, phone_number) VALUES 
(1, 'Bruce Willis', 'barjam@hotmail.com', '2016-07-05', 'o8sdffsmgtswxjvxxl31', '+353 20 912 2322'),
(2, 'George Clooney', 'tellis@me.com', '2016-02-22', 'sx8pav3ggtvfwdz1yte7', '+353 20 912 2323'),
(3, 'Kevin Costner', 'metzzo@hotmail.com', '2016-03-26', 'l51q47urv4hbqqa5f87g', '+353 20 912 2324'),
(4, 'Donald Sutherland', 'ralamosm@verizon.net', '2016-11-03', 'pj2625765oehrlpk6lo4', '+353 20 912 2325'),
(5, 'Jennifer Lopez', 'barjam@hotmail.com', '2016-03-02', 'c70n1nz39ggc9881ybst', '+353 20 912 2326'),
(6, 'Ray Liotta', 'jdhedden@comcast.net', '2017-02-24', 'qpnuvi7mndgl1qmxgdl1', '+353 20 912 2327'),
(7, 'Samuel L. Jackson', 'moonlapse@outlook.com', '2018-07-19', 'i6yvht95527z3idgqx9y', '+353 20 912 2328'),
(8, 'Nikole Kidman', 'okroeger@msn.com', '2016-09-17', '3bhg1l720u1reugsmbfc', '+353 20 912 2329'),
(9, 'Alan Rickman', 'karasik@verizon.net', '2016-10-03', '86ezqmymrhof0w81x3n9', '+353 20 912 2330'),
(10, 'Kurt Russell', 'gator@live.com', '2016-08-18', '4wwzx2kpn81410q79ieh', '+353 20 912 2331'),
(11, 'Harrison Ford', 'kostas@hotmail.com', '2016-12-05', 'u8sxb8byhaajee65n9t2', '+353 20 912 2332'),
(12, 'Russell Crowe', 'glenz@att.net', '2018-01-04', 'ywtkc8tns9le6aioalyf', '+353 20 912 2333'),
(13, 'Steve Martin', 'nelson@outlook.com', '2016-07-29', 'w76yphg3kvzg77ilmxfs', '+353 20 912 2334'),
(14, 'Michael Caine', 'dmouse@live.com', '2016-04-24', '7k6m698ky9de34yc9zrh', '+353 20 912 2335'),
(15, 'Angelina Jolie', 'chance@att.net', '2018-06-22', 'f403jj1cpkzoiwicn0kz', '+353 20 912 2336'),
(16, 'Mel Gibson', 'rohitm@yahoo.ca', '2016-01-02', 'hojjtsy7rt0v7we42vlr', '+353 20 912 2337'),
(17, 'Michael Douglas', 'timtroyr@hotmail.com', '2016-08-02', '03ga9r324u8n25ujb5ue', '+353 20 912 2338'),
(18, 'John Travolta', 'wainwrig@msn.com', '2016-11-19', 'fzjhl0v82o0amalr8649', '+353 20 912 2339'),
(19, 'Sylvester Stallone', 'kohlis@aol.com', '2018-10-04', 'b26226km8w1qfzqpi9so', '+353 20 912 2340'),
(20, 'Tommy Lee Jones', 'szymansk@live.com', '2018-03-09', 'c46s9eodm9k3qiwvju3y', '+353 20 912 2341'),
(21, 'Catherine Zeta-Jones', 'flakeg@hotmail.com', '2016-04-02', 'izq356fwuzdhc6u1skan', '+353 20 912 2342'),
(22, 'Antonio Banderas', 'sassen@verizon.net', '2018-03-23', 'wftjnqkjfqi7dj7g6oeo', '+353 20 912 2343'),
(23, 'Kim Basinger', 'jaesenj@sbcglobal.net', '2017-09-27', 'h60m7wovjopzp9kx4m3m', '+353 20 912 2344'),
(24, 'Sam Neill', 'clkao@live.com', '2017-02-05', '3rpgiccs25fj7apg246s', '+353 20 912 2345'),
(25, 'Hideo Kojima', 'admin@sql-academy.org', '2017-03-08', '97shpolky5vg3b2qn2wu', '+353 20 912 2346'),
(26, 'ClINT Eastwood', 'froodian@verizon.net', '2019-02-10', 'ogbjpnp7vlzwxu4bj0bs', '+353 20 912 2347'),
(27, 'Brad Pitt', 'kewley@optonline.net', '2017-02-11', '829j2ygocn8btzae49kv', '+353 20 912 2348'),
(28, 'Johnny Depp', 'cgarcia@yahoo.ca', '2017-05-26', 'qpp6hbnae42cdhmxlk4j', '+353 20 912 2349'),
(29, 'Pierce Brosnan', 'treeves@icloud.com', '2019-03-08', 'lqiwecclne9rv8woo2go', '+353 20 912 2350'),
(30, 'Sean Connery', 'jschauma@icloud.com', '2016-05-21', 'lyh4jkdxkvtvulvqi5db', '+353 20 912 2351'),
(31, 'Bruce Willis', 'kewley@icloud.com', '2016-12-08', '0ofa2khvnptiackbssv0', '+353 20 912 2352'),
(32, 'Mullah Omar', 'jgoerzen@me.com', '2019-07-18', 'f3ft4fwo7vafvqb0ugk5', '+353 20 912 2353'),
(33, 'Vasanta Roberta', 'roberta@me.com', '2017-08-11', 'f3ftsdfsdffvqb0ugk5', '+353 20 912 2354');
