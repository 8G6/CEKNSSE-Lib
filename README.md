# CEKNSSE-
RED='\033[01;31m'
echo -e "${RED} Bash Code By DSB"
figlet RYU CODER
YELLOW='\033[01;33m'                                         
CYAN='\033[01;36m'                                           
echo -e "        ${CYAN}This is bash scrpting"
echo -e "This script will install all dependences for notebook"
echo -e "${RED} Updating and upgrading"
pkg update && pkg upgrade
echo-e "${RED}instaling clang for c/c++"
echo -e "\e[0m"
pkg install clang
echo -e "${RED} installing python "
pkg install  python
echo -e "${RED}installing fftw"
echo -e "\e[0m"
pkg install fftw 
echo -e "${RED}installing main lib"
echo -e "\e[0m"
pkg install libzmq 
echo -e "${RED}installing main freetype"
echo -e "\e[0m"
pkg install freetype 
echo -e "${RED}installing png libray"
echo -e "\e[0m"
pkg install libpng
echo -e "${RED}Setting up env"
LDFLAGS="-lm -lcompiler_rt" 
echo -e "${RED}installing jupyter notebook"
echo -e "\e[0m"
pip install jupyter 
echo -e "${RED}Testing notebook"
echo -e "${YELLOW}If notebook launched sucess you can see some thing like this ${CYAN}To access the notebook, openlike this file in a browser:"
jupyter notebook
