# sublist3r
virustotal_fixed

SET UP

1. $ sudo apt-get install sublist3r

2. Register and get the virustotal API key.(premium key is not a must)

3. $ git clone https://github.com/cybersecinvestigators/sublist3r.git

4. $ cd sublist3r/

5. $ nano sublist3r.py

6. go to line number 688 (ctrl+shift+_)

7. Place your virustotal API key in line number 688 in this python script => resp = self.session.get(url, headers={"x-apikey":"Your_API_KEY"}, timeout=self.timeout)

8. Replace the Original sublist3r.py file with this.

    $ sudo cp sublist3r.py /usr/lib/python3/dist-packages/sublist3r.py

USAGE

sublist3r -d domain.com

