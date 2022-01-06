Code for my website, at https://feiwangyuzhou.github.io.
It is a fork from raihanjoty's at https://raihanjoty.github.io




#Generate papers

```

python scripts/parsebib.py papers/bibtex.bib  2>/dev/null  | perl -anpe 's/\t/    /g;' > _data/papers.yml

```

#Create individual pages for papers

```

python scripts/migrate.py _data/papers.yml  

```
