# /*******************************************************************************
#  Copyright (C) 2021 Xilinx, Inc
#
#  Licensed under the Apache License, Version 2.0 (the "License");
#  you may not use this file except in compliance with the License.
#  You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
#  Unless required by applicable law or agreed to in writing, software
#  distributed under the License is distributed on an "AS IS" BASIS,
#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#  See the License for the specific language governing permissions and
#  limitations under the License.
#
# *******************************************************************************/

TARGET=ip
DEVICE=xcu250-figd2104-2L-e
DTYPES=float half double int32_t int64_t
DWIDTH=512
REDUCE_IP = reduce_sum.xo

all: $(REDUCE_IP)

reduce_sum.xo: build.tcl reduce_sum.cpp
	vitis_hls $< -tclargs $(TARGET) $(DEVICE)


