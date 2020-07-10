# Programming-FPGA-Basys3-with-VHDL
VHDL 
library IEEE;
use IEEE.std_logic_1164.all;
use IEEE.numeric_std.all;
use IEEE.std_logic_unsigned.all;
entity masterswitch is
Port (Msw: in std_logic;
sw1: in std_logic;
sw2: in std_logic;
LED1: out std_logic;
LED2: out std_logic );
end masterswitch;
architecture Behavioral of masterswitch is
begin
LED1 <= Msw And sw1;
LED2 <= Msw And sw2;
end Behavioral;
